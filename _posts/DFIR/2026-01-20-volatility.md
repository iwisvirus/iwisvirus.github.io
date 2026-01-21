---
layout: post
title: TryHackMe | Volatility
date: 2026-01-20
categories: DFIR
---

Volatility is a forensic tool commonly used by SOC analysts within the blue team. It is written in python.
It is widely used for extracting digital artificats from volatile memory(RAM) samples. For this module, 
I downloaded files for the test runs. I got python, Pefile, and a file from this link  <br>

[(https://github.com/volatilityfoundation/volatility3/releases/tag/v1.0.1)]

These are the tools that can be used to extract a memory from a metal machine 
- FTK imager
- Redline
- Dumplt.exe
- wind32dd.exe
- Memoryze
- FastDump
And these tools usually output a .raw file.

__PLUGINS__
**windows.info/linux.info/mac.info**: information about what the host is running from the memory dump 
 - python3 vol.py -f <file> windows.info : provide information about the host from memory dump

**imageinfo** : take provided memory dump and assign it a list of the best possible OS profiles

**pslist**: get list of processes from the doubly-linked list that keeps track of processes in memory, equivalent to the process list in task manager. include all current processes and terminated process with their exit time 
- python3 vol.py -f <file> windows.pslist

**psscan**: locate processes by finding data structures that match _EPROCESS. It can cause false positives. good to detect unlinked malwares that doesn't show up on pslist
- python3 vol.py -f <file> windows.psscan

**pstree**: list all processes based on their parent process ID, using the same methods as pslist. Useful to get a full story of the processes and what may have been occurring at the time of extraction 
- python3 vol.py -f <file> windows.pstree

**netstat**: attempt to identify all memory structures with a network connection 
- python3 vol.py -f <file> windows.netstat

**dlllist**: list all DLLs associated with processes at the time of extraction. useful once you have done further analysis and can filter output to a specific DLL that might be an indicator for a specific type of malware you believe to be present on the system
- python3 vol.py -f <file> windows.dlllist

**malfind**: useful when hunting for code injection. attempty to identify injected processes and their PIDs along with the offset address and a Hex, Ascii, and Disassembly view of the infected area. Works by scanning the heap and identifying processes 
- python3 vol.py -f <file> windows.malfind

**yarascan**: search for strings, patterns, compound rules against a rule set. Can use a YARA file as an argument or list rules within the command line 
- python3 vol.py -f <file> windows.yarascan

**INVASION TECHNIQUE**
**Hooking**
- SSDT(System Service Descriptor Table)
  - Most common
  - searches for hooking and output its results
  - Window kernel uses this table to look up system functions
  - adversay can hook into this table and modify pointers to point to a location the rootkit controls
  - python3 vol.py -f <file> windows.ssdt 
- IRP
- IAT
- EAT
- Inline

**PLUGINS**
**Module**: dump a list of loaded kernel modules. useful in identifying active malware 
- python3 vol.py -f <file> windows.modules

**driverscan**: scan for drivers present on the system at the time of extraction. identify driver files in the kernel. prior investigation before using the plugin 
- python3 vol.py -f <file> windows.driverscan

**modscan, driverirp, callbacks, idt, apihooks, moddump, handles**


These are some practical investigations using what I've learned. 
**1. What is the build version of the host machine in Case001? (2600.xpsp.080413-2111)** <br>

For this task, I used 
**python3 vol.py -f <file> windows.info**
![PDF Info Screenshot]({{ site.baseurl }}/images/vol1.png)

**2. At what time was the memory file acquired in Case 001?(2012-07-22 02:45:08)** <br>

For this task, I used 
**python3 vol.py -f <file> windows.info**
![PDF Info Screenshot]({{ site.baseurl }}/images/vol2.png)

**3.What process can be considered suspicious in Case 001?(reader_sl.exe)** <br> 

For this task, I used
**python3 vol.py -f <file> windows.psscan**
![PDF Info Screenshot]({{ site.baseurl }}/images/vol3.png)

**4.What is the parent process of the suspicious process in Case 001?(explorer.exe)** <br>

For this task, I used
**python3 vol.py -f <file> windows.pstree**
![PDF Info Screenshot]({{ site.baseurl }}/images/vol4.png)

**5.What is the PID of the suspicious process in Case 001?(1640)** <br>

For this task, I used
**python3 vol.py -f <file> windows.cmd**

**6.What is the parent process PID in Case 001?(1484)**

For this task, I used
**python3 vol.py -f <file> windows.cmd**

**7.What user-agent was employed by the adversary in Case 001?(Mozilla/5.0(Windows;U;MSIE 7.0;Windows NT 6.0; en-US))**

For this task, I used 
**python3 vol.py -f <file> -o <file to save> windows.memmap.Memmap --pid 1640 --dump**
![PDF Info Screenshot]({{ site.baseurl }}/images/vol5.png)

then, 

**python3 vol.py -f <file>/*.dmp | grep -i "user-agent"**
![PDF Info Screenshot]({{ site.baseurl }}/images/vol6.png)

**8.Was Chase Bank one of the suspicious bank domains found in Case 001? (Y/N) (Y)**

For this task, I used
**python3 vol.py -f <file>/*.dmp | grep -i "chase"**
![PDF Info Screenshot]({{ site.baseurl }}/images/vol7.png)

**9.What suspicious process is running at PID 740 in Case 002?(@WanaDecryptor@)**

For this task, I used
**python3 vol.py -f <file>/ windows.psscan"**
![PDF Info Screenshot]({{ site.baseurl }}/images/vol8.png)


**10.What is the full path of the suspicious binary in PID 740 in Case 002?(C:\Intel\ivecuqmanpnirkt615\@WAnaDecryptor@)**

For this task, I used
**python3 vol.py -f <file>/*.dmp windows.dlllist | grep 740**
![PDF Info Screenshot]({{ site.baseurl }}/images/vol9.png)

**11.What is the parent process of PID 740 in Case 002?(tasksche.exe)**

For this task, I used
**python3 vol.py -f <file>/*.dmp windows.pstree**
![PDF Info Screenshot]({{ site.baseurl }}/images/vol10.png)

**12.What is the suspicious parent process PID connected to the decryptor in Case 002?(1940)**

For this task, I used
**python3 vol.py -f <file>/*.dmp windows.pstree"**

**13.From our current information, what malware is present on the system in Case 002?(Wannacry)**

I had to search this up on the internet. 

**14.What DLL is loaded by the decryptor used for socket creation in Case 002?(Ws2_32.dll)**

I had to search this up on the internet. 

**15.What mutex can be found that is a known indicator of the malware in question in Case 002?(MsWinZonesCacheCounterMutexA)**

For this task, I used
**python3 vol.py -f <file>/*.dmp windows.handles | grep 1940**
![PDF Info Screenshot]({{ site.baseurl }}/images/vol11.png)

**16.What plugin could be used to identify all files loaded from the malware working directory in Case 002?(windows.filescan)**

For this task, I used the help menu. 
![PDF Info Screenshot]({{ site.baseurl }}/images/vol12.png)









