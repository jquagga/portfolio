---
title: "Jupyter Notebook meets SDR data about a P25 system"
excerpt: "This notebook was part of a personal project where SDRs monitor the county's public radio network. <br/><img src='/images/p25.png'>"
collection: portfolio
---

One project I maintain is a simple tool which takes audio from the excellent [Trunk-Recorder](https://github.com/TrunkRecorder/trunk-recorder) and runs it through Whisper.ai to produce text transcripts. Basically [pwcscanner.org](https://www.pwcscanner.org) is the same police and fire scanner your dad had, except you can read semi-accurate text transcripts of what is going on.

As part of this task, I wanted to gauge how many "calls" my system could handle. For example, I don't transcribe what the school busses are saying, but generally I'm curious about what police or fire might be doing. "Where are all those sirens going?". Trunk recorder keeps a log of all of its calls and generally, what it did them. Was the call encrypted and thus, un-recordable? Was it in a talkgroup I don't follow or perhaps it was excluded? And also, just how many calls were there overall?

I put together a simple Python script which morphed into a Jupyter lab product that uses regex to parse the text, sort the calls into categories and provide some context of just what is going on. The code to the project is [on github](https://github.com/jquagga/tr-log-analyzer) however if you aren't actively monitoring a system and have logs, please take a look at [at this file](/assets/trlog.html) for all sort of interesting data.
