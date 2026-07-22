---
layout: post
title: DRL | How to find out if a video was surpressed or a altered
date: 2026-07-22
categories: DFIR
---

How do we find out if a video was surpressed or altered?

1. Confirm what's in the file you have
  - in powershell you can run
    ffprob -v error -show_entries stream=index, codec_type, code_name "C:\path\to\file.avi"
  - the code_type shows if it is video or audio
2. you have to get the original .dav files since .avi files are conversions.
3. test drive the .dav files for audio
  - play them in Dahua SmartPlayer or use
    ffprob -v error -show_entries stream=codec_type, codec_name "C:\path\to\file.dav"
  - if audio exist, there is a second stream pcm_alaw or pcm_mulaw

- make sure the files are zipped so that the original metadata is preserved
- make sure you get the .dav file not the .avi file
- 

