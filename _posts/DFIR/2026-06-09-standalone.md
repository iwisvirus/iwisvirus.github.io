---
layout: post
title: PCE | Standalone System
date: 2026-06-09
categories: DFIR
---

**types of pw located in registry and user profiles**

- registry and user profile directories store
  - windows configuration info, pw, other login data for installed applications
![PDF Info Screenshot](/images/standalone1.png)

![PDF Info Screenshot](/images/standalone2.png)

**Standalone system analysis**

- all users, adminstrator, guest, defaultaccount, WDAGutilityaccount, dmitry

**Windows Hello**
- sometimes recover user pw
- when specifying a path to the config folder in passware kit, make sure that folder microsoft is present alongside the config folder, similar to its arrangement in the system32 folder in windows
![PDF Info Screenshot](/images/standalone3.png)
![PDF Info Screenshot](/images/standalone4.png)

- for tpm protected machines, its possible to recover pw for local windows acccounts with enabled windows hello options using regular brute force and rainbow tables methods, regardless of live id
![PDF Info Screenshot](/images/standalone5.png)




