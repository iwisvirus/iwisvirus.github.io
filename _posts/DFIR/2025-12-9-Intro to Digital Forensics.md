---
layout: post
title: TryHackMe | Intro to Digital Forensics
date: 2025-12-09
categories: DFIR
---

Today, I went through the introduction course and learned how to retrieve pdf and jpg information using command functions in the terminal. We can retrieve information about a pdf using “pdfinfo” command line like the picture below. It shows the title, name of the person who wrote, date, number of pages, and so on. 

![PDF Info Screenshot]({{ site.baseurl }}/images/image1_intro.jpg)

Then I tested it on a pdf that I already have on my computer. It was interesting to see that they know it’s written on LaTex. 

![PDF Info Screenshot]({{ site.baseurl }}/images/intro2.png)


We can also retrieve information about a jpg using “exiftool” command. Some interesting thing I noticed is that you can see what the picture was taken with, if the flash was on or off, exposure time, and file permission. 

![PDF Info Screenshot]({{ site.baseurl }}/images/intro3.png)

I also tested it on a jpg image I have on my computer. 

![PDF Info Screenshot]({{ site.baseurl }}/images/intro4.png)
