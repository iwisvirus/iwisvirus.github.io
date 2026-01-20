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






![PDF Info Screenshot]({{ site.baseurl }}/images/image1_intro.jpg)








