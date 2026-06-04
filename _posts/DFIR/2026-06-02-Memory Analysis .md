---
layout: post
title: PCE | Memory Analysis
date: 2026-06-02
categories: DFIR
---

**Volatile Memory**
- applications and operating systems store pw in volatile memory
- passware kit forensic analyzes memory dumps for pw and account details & extracts encryption keys and in some cases, passwords and other user account details from volatile memory
- data is only stored in memory while the device is powered on
- memory capture should be done at the point of seizure

**Passware Bootable Memory Imager**
- useful since many encryption applications store pw and keys in RAM
- passware kit can analyze and extract some of them from  memory image
- passware kit can create custom dictionary from memory image
- can be used against hard drives encrypted with bitlocker TPM protector or APFS/FileVault without T2 chip inside
- supported OS: Windows, Linux, macOS
- PBMI does not support Macs with T2/M1/M2 chips inside
- acquires memory image after a warm boot of the target machine 
