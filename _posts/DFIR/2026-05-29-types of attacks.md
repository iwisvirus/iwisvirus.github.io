---
layout: post
title: PCE | Types of Attacks
date: 2026-05-29
categories: DFIR
---

Basic attacks
  - dictionary
      - pre defined list of possible pw
      - modifiers increase number of tested pw and usd to change case type, character order, and subtitute characters in pw candidates
  - zieve
      - skips nonsensical combination of characters
      - range of pw length, character set language, symbol set, custome characters, pattern, xieve level, modifiers all customizable 
  - brute-force
      - thorough but slow
  - mask
      - "matches a specified pattern"
      - uses a mask to filter down possible pw
      - ?l(lower), ?u(upper), ?d(num), ?h(num abcdef), ?H(num,ABCDEF), ?s(symbol), ?a(?l?u?d?s)
  - known pw/part
      - check a single pw or a short list of known pw
      - no need to create a custom dictionary to check a short list of pw
      - most commonly used a join attacks group
      - modifiers can be applied
      - can be used as a part of a more complex attack
      - can check if a pw is correct without having to open the file or create a decrypted image of the encrypted volume 
  - previous pw

group
  - join attacks
  - append attacks

special
  - encryption keys extraction
      - only one microsoft words, excel, powerpoint 2007-2019
      - decrypt file instantly 
  - zip plaintext
      - win zip encryption
  - rainbow tables
      - password hashes, microsoft for certain years
      - set of pre computer hashes
      - can look up what hashes would make up that password 
  - surezip
      - at least simultaneously 5 encrypted files 

- attack settings
- recovery process can be paused, stopped, and resumed
- recovery process can be saved and exported to be resume on other machines



![PDF Info Screenshot](/images/pce1.png)
