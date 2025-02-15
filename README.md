# Crash Bandicoot Resources

This repository was made to collect all the resource about crash bandicoot file format, related reverse engineer studies and tools, feel free to contribute with fork + pull request.


## Crash Bandicoot N Sane Trilogy (CB NST)

CBNST is composed by **file.pak** that are archives, can we open/edit it? Yes! We can use NeoKesha's tool, [NeoKesha's tool, PAK Explorer](http://twinsanity-hacking.tigersoftware.ru/viewtopic.php?f=2&t=6075) , it allows to extract the content, modify the position of the file, repack and create new patch.

Little example [here](https://www.youtube.com/watch?v=ArDcqoyF7iA), this video show how to swap the models and repack, indeed, at the end of the video we can see a scene of Crash Bandicoot where the 3D models (**file.igz**) of the evil characters are swapped with the bandicoot characters.

NST PAK Explorer allows to extract the file but one by one, to extract automatically all the archive we can use the [Aluigi's tool Quickbms](http://aluigi.altervista.org/quickbms.htm) Aluigi's tool Quickbms and the related script compatible with CBNST.

**Problem**: we still can't open the .igz files, [here](https://www.vg-resource.com/thread-32408-page-4.html)  there are some users that are working on it, they will give updates on that thread.
I found on github a tool that can convert file .igz into .pvr file but I don't know really if it works properly.

### Tools CBNST

- **NST PAK Explorer** [github](https://github.com/NeoKesha/NST_Explorer) [download](https://yadi.sk/d/0Ytfg3ca3YjtTN) [reference](http://twinsanity-hacking.tigersoftware.ru/viewtopic.php?f=2&t=6075) [video](https://www.youtube.com/watch?v=ArDcqoyF7iA)
- **Quickbms** [download](http://aluigi.altervista.org/quickbms.htm)
- **Quickbms script** [download](http://aluigi.altervista.org/bms/marvel_ultimate_alliance_2.bms) [reference](http://zenhax.com/viewtopic.php?t=7794)
- **IGZ Editor** [download](https://yadi.sk/d/6ofo5uq_3YpLV6) [reference](http://twinsanity-hacking.tigersoftware.ru/viewtopic.php?f=2&t=6076) [video](https://www.youtube.com/watch?v=1eiHJmjZrks)
- **Crash-Bandicoot-NSAMETRIOLOGY-Tool** [download](https://github.com/pashok6798/Crash-Bandicoot-NSAMETRIOLOGY-Tool)
-  **ARD's Texture Converter** [reference & download](https://thewarproom.com/showthread.php?tid=27)
- **ARD's Level Editor prototype** [reference](https://thewarproom.com/showthread.php?tid=32)
- **ARD'S Level Selector** [reference](https://thewarproom.com/showthread.php?tid=44) [download](https://www.mediafire.com/file/m1ff4b313nakax0/NSTLevelSelector.exe)
- ~IGZ Model Converter~ deprecated for igModelConverter [github](https://github.com/AdventureT/igModelConverter), related QT GUI project [github](https://github.com/AdventureT/IgzModelConverterQT)

**For Linux users?** These tools are compatible with Windows, but they work pretty good with wine/mono, about quickbms it works, but there is also the source code available.

[PAK & IGZ file format structure](https://thewarproom.com/showthread.php?tid=8)

### CBNST Mods Released
**Level Mod by ARD** [guide & download](https://thewarproom.com/showthread.php?tid=21)
**Crash Classic Soundtrack** [guide & download](https://cogmonkey.com/CrashNSTOST/)

### Character Mods
- **Skeleton Crash** [download](https://www.nexusmods.com/crashbandicootnsanetrilogy/mods/1) 
- **Low-poly Crash** [download](https://www.nexusmods.com/crashbandicootnsanetrilogy/mods/2)
- **Fake Crash** [download](https://www.nexusmods.com/crashbandicootnsanetrilogy/mods/3)
- **Biker Crash** [download](https://www.nexusmods.com/crashbandicootnsanetrilogy/mods/6)
- **Jetpack Crash** [download](https://www.nexusmods.com/crashbandicootnsanetrilogy/mods/7)
- **Pilot Crash** [download](https://www.nexusmods.com/crashbandicootnsanetrilogy/mods/8)
- **Scuba Crash** [download](https://www.nexusmods.com/crashbandicootnsanetrilogy/mods/9)
- **Boxers Crash** [download](https://www.nexusmods.com/crashbandicootnsanetrilogy/mods/10)

### Interesting projects about CBNST
- **ReBandicoot**, this project is attempting to reverse engineer the CBNST game [github](https://github.com/2010kohtep/ReBandicoot)
- **Insan3Mod** modtools for CBNST [github](https://github.com/dtzxporter/Insan3Mod)
- **CrashBandicootGodot**: Crash bandicoot mechanics in godot [github](https://github.com/nonunknown/crash-bandicoot-godot)
 
---

### Crash Twinsanity
- NeoKesha's **Crash Twinsanity Editor** [github](https://github.com/Smartkin/twinsanity-editor), [reference](http://twinsanity-hacking.tigersoftware.ru/viewtopic.php?t=2), [youtube](https://www.youtube.com/watch?v=eBE51p8zAlU)
- OpenSanity: decompile Crash Twinsanity [github](https://github.com/NeoKesha/OpenSanity)
- Twinsanity script reader [github](https://github.com/Smartkin/twinsanity-script-reader)
- Twinsanity-reversed: old project about crash twinsanity decopmilation [github](https://github.com/Smartkin/twinsanity-reversed)
- OpenSanityNeo: Crash Twinsanity (XBOX PAL) decompilation\disassembly project [github](https://github.com/NeoKesha/OpenSanityNeo)

---

### Crash Team Racing

[CTR-tools](https://github.com/CTR-tools)
This organization includes some tools to edits/explore the CTR levels and also to unpack partially the CrashBash.DAT file.

---

### Crash Bash  

The tool [CTR-tools](https://github.com/CTR-tools) is able to extract all files (textures, music etc.) from multiple crash bash versions.  
[CrashBashEx](https://github.com/xan1242/CrashBashEx) can extract some Crash Bash music data from the CRASHBASH.DAT file.  
Another tool related to Crash Bash is in the section below `Crash Bandicoot & AI`.  

[Arbitrary Code Execution (ACE) in Crash Bash NTSC-J ](https://github.com/lazycurler/CrashBashResearchACE) -> speed run the game using some specific inputt cheat that changes the crash bash memory.
Better explanation and related video is available [here](https://github.com/lazycurler/CrashBashResearchACE#links).

---


## Crash Bandicoot Trilogy (PS1)

The Crash Bandicoot Trilogy games are composed by ***.NSD, *.NSF** file how to get them?
If you have the **Game.cdz** you can convert it to Game.bin with psxfin or cdztool (PSX tool included in the emulator) and then to Game.iso with ccd2iso if you use Linux/Mac or with [these tools](https://helpdeskgeek.com/free-tools-review/how-to-convert-bin-to-iso/) if you use Windows.
When you have the iso file you can easily extract it and get the NSD/NSF files.

When you have the NSD/NSF files you can open them with the tool **CrashEdit** or **drnsf**, the former allows to edit, play/export the sound file, the texture etc. the latter, allows to open the nsd/nsf file and view the 3D models.
**Drnsf** don't export the 3D models, while the last version of CrashEdit should allows to export the scenery 3d model.

Another tool that export the 3D models is **[Crash-Bandicoot-2-Modelexport](https://github.com/warenhuis/Crash-Bandicoot-2-Modelexport)** but it depends on CrashEdit as you can see in [this video](https://www.youtube.com/watch?v=g7ByLSotvNo).

A simple tool (for developers mainly) that only "load" the nsf file in memory and start to work on them could be [crash-bandicoot-nsf](https://github.com/dehodson/crash-bandicoot-nsf), is a simple python script to read the nsf file, you can use it to study how this kind of programs works and maybe write a new one.

---

## Crash Bandicoot & AI

**Crash Bash AI** for "Crashball level" winrate 100% using Reinforcement Learning. 
[source](https://mobile.twitter.com/theredhotbr/status/1272643329327542277), 
[video](https://clips.twitch.tv/InnocentFineAardvarkTheThing), 
[GitHub repository](https://github.com/mateusfavarin/RillAi)

**Crash Team Racing** AI to recognize the time in game of a speedrun.
[Github Repository](https://github.com/mateusfavarin/CTR-AutoIGT)

---

### Wiki & website
[cbhacks](https://www.cbhacks.com/)  
[cbhacks wiki](https://wiki.cbhacks.com/w/Main_Page)  

---

### Tools
- **psxfin**, **cdztool**, **ccd2iso**
- **CrashEdit** [download](https://github.com/ManDude/CrashEdit/) (deprecated, use drnsf)
- **Crash-Bandicoot-2-Modelexport** [download](https://github.com/warenhuis/Crash-Bandicoot-2-Modelexport) [reference](https://www.youtube.com/watch?v=g7ByLSotvNo)
- **drnsf** [download](https://github.com/cbhacks/drnsf) 
- **crash-bandicoot-nsf** [download](https://github.com/dehodson/crash-bandicoot-nsf) 
- **goocdump** [download](https://github.com/ManDude/goocdump), GOOL -> GOOC converter. 

---
### Other
- **Crash 2 engine in C** [github page](https://github.com/ughman/c2c)
- **Crash 1 engine in C** [github page](https://github.com/wurlyfox/c1)
- **Tools for Crash Bandicoot Mutant Island 2008 Java game** [download](https://github.com/bartlomiejduda/Tools/tree/master/NEW%20Tools/Crash%20Bandicoot%20Mutant%20Island%202008)
- **crash-bandicoot-godot** [download](https://github.com/nonunknown/crash-bandicoot-godot) 
- **OpenCrashWOC** [download](https://github.com/Open-Travelers/OpenCrashWOC) 
- **Ray1Map** to check the maps of Vicarious Visions Crash GBA games, try [live demo here](https://raym.app/maps_r1).
 
