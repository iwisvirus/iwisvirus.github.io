---
layout: post
title: TryHackMe | Unattended - Practice
date: 2026-01-22
categories: DFIR
---

Today, I did a practice lab for Windows Forensics and the basic tools I've learned throughout the past month. 

Case: There is a employee that was newly hired who saw a suspicious-looking janitor exiting his office as he was about to return from lunch. 
We will be investigating if there was user activity while the user was away between **12:05PM to 12:45PM on the 19th November 2022**. 

The initial investigation shows that there was someone who accessed the computer during the previously specificed timeframe. 
**1. What file type was searched for using the search bar in Windows Explorer?** <br> 

I used the registry explorer tool to tackle this problem. 

![PDF Info Screenshot]({{ site.baseurl }}/images/test1.png)

**2. What top-secret keyword was searched for using the search bar in Windows Explorer?** <br>

I used the registry explorer tool to tackle this problem as well. 

![PDF Info Screenshot]({{ site.baseurl }}/images/test2.png)

**3. What is the name of the downloaded file to the Downloads folder?** <br>

I used the Autopsy tool and looked through the Downloads file to tackle this problem 
![PDF Info Screenshot]({{ site.baseurl }}/images/test3.png)

**4. When was the file from the previous question downloaded?**

I used the Autopsy tool and looked through the Downloads file to tackle this problem 
![PDF Info Screenshot]({{ site.baseurl }}/images/test4.png)

**5. Thanks to the previously downloaded file, a PNG file was opened. When was thihs file opened?**

I used the registry explorer tool to tackle this problem. When you right click the file, there's actually a tool that gives you all the details which I found very helpful.

![PDF Info Screenshot]({{ site.baseurl }}/images/test5.png)
![PDF Info Screenshot]({{ site.baseurl }}/images/test6.png)

**6. A text file was created in the Desktop folder. How many times was this file opened?**

I used the command prompt with the JLECmd.exe tool.
![PDF Info Screenshot]({{ site.baseurl }}/images/test7.png)

**7. When was the text file from the previous question last modified?**

I used the command prompt with the JLECmd.exe tool.
![PDF Info Screenshot]({{ site.baseurl }}/images/test7.png)

**8. The contents of the file were exfiltrated to pastebin.com. What is the generated URL of the exfiltrated data?**

I used the Autopsy tool and looked through the web history. 
![PDF Info Screenshot]({{ site.baseurl }}/images/test8.png)


**9. What is the string that was copied to the pastebin URL?**

I used the Autopsy tool and looked through the web history. 
![PDF Info Screenshot]({{ site.baseurl }}/images/test9.png)


Summary:

Finding what I need inside the tool is quite easy. The tricky part for me was choosing the right tool for each task. I might have to review on that to know exactly what tool I need to solve a problem. 
