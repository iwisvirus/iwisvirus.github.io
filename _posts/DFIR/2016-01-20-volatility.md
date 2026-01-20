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



![PDF Info Screenshot]({{ site.baseurl }}/images/image1_intro.jpg)

Then I tested it on a pdf that I already have on my computer. It was interesting to see that they know it’s written on LaTex. 

![PDF Info Screenshot]({{ site.baseurl }}/images/intro2.png)


We can also retrieve information about a jpg using “exiftool” command. Some interesting thing I noticed is that you can see what the picture was taken with, if the flash was on or off, exposure time, and file permission. 

![PDF Info Screenshot]({{ site.baseurl }}/images/intro3.png)

I also tested it on a jpg image I have on my computer. 

![PDF Info Screenshot]({{ site.baseurl }}/images/intro4.png)
