---
layout: post
title: Frankwxu | Number Systems & Timestamps
date: 2026-01-23
categories: DFIR
---


Today, I learned number systems and timestamps. 

**Number Systems**

|  System  |  Humans  |   CPU    | Forensics|
|----------|----------|----------|----------|
|  Decimal |     Y    |     N    |     Y    |
|  Binary  |     N    |     Y    |     Y    |
|   Hexa   |     N    |     N    |     Y    |

**American Standard Code for Information Interchange**
 __ASCII vs UTF-8__
- both are character encoding standards used for representing characters (letters, numbers, symbols, series of bits)
- length difference
  - ASCII : 7 bits
  - UTF-8 : variable-length encoding
- UTF-8 is a superset of ASCII
  - all ASCII characters have same representation in UTF-8
  - UTF-8 can represent a wider range of characters, including non-English characters

**Epoch time and timestamps**
- way to represent time as the number of seconds/milliseconds that have passed since a specific starting point
  - 1 sec = 1000 milliseconds (ms) = 1000000 microseconds(us)
- types
  - Unix Epoch (POSIX)
    - describing points in time, number of seconds that have elasped since the Unix epoch where it is 00:00:00 UTC on 1,1, 1970
  - Mac Time : Mac OS X time/cocoa core date, HFS+/APFS
    - epoch date for mac is midnight 1,1, 2001 and cocoa core data time is the number of seconds elasped since 1,1, 2001 00:00:00 UTC
    - difference in 31 years 
  - WebKit time
    - rendering engine used by web browsers (Safari, Google Chrome)
    - time it takes for the WebKit rendering engine to render and display a webpage
    - webkit microsecond since 1,1,1601
  - Windows Filetime

**Data stored in memory**
__Endianness__
- term that describe the order in which a sequence of bytes is stored in memoory
- little-endian : order in which the little end(least significant value in the sequence) is stored first
- big-endian : order in which the big end(most significant value in the sequence) is stored first 

