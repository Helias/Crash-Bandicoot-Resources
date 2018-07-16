# Crash Bandicoot Resources

This repository was made to collect all the resource about crash bandicoot file format and related reverse engineer studies and tools.


## Crash Bandicoot N Sane Trilogy (CB NST)

CBNST is composed by **file.pak** that are archives, can we open/edit it? Yes! We can use NeoKesha's tool, [NeoKesha's tool, PAK Explorer](http://twinsanity-hacking.tigersoftware.ru/viewtopic.php?f=2&t=6075) , it allows to extract the content, modify the position of the file, repack and create new patch.

Little example [here](https://www.youtube.com/watch?v=ArDcqoyF7iA), this video show how to swap the models and repack, indeed, at the end of the video we can see a scene of Crash Bandicoot where the 3D models (**file.igz**) of the evil characters are swapped with the bandicoot characters.

NST PAK Explorer allows to extract the file but one by one, to extract automatically all the archive we can use the [Aluigi's tool Quickbms](http://aluigi.altervista.org/quickbms.htm) Aluigi's tool Quickbms and the related script compatible with CBNST.

**Problem**: we still can't open the .igz files, [here](https://www.vg-resource.com/thread-32408-page-4.html)  there are some users that are working on it, they will give updates on that thread.
I found on github a tool that can convert file .igz into .pvr file but I don't know really if it works properly.

[Crash-Bandicoot-NSAMETRIOLOGY-Tool](https://github.com/pashok6798/Crash-Bandicoot-NSAMETRIOLOGY-Tool) (author: Pashok6798)
I compiled on Linux with xbuild/mono and I tried it, but I didn't know how to open .pvr file so I can't test it.


### Tools summary CBNST

- **NST PAK Explorer** [download](https://yadi.sk/d/0Ytfg3ca3YjtTN) [reference](http://twinsanity-hacking.tigersoftware.ru/viewtopic.php?f=2&t=6075)
- **Quickbms** [download](http://aluigi.altervista.org/quickbms.htm)
- **Quickbms script** [download](http://aluigi.altervista.org/bms/marvel_ultimate_alliance_2.bms) [reference](http://zenhax.com/viewtopic.php?t=7794)
- **Crash-Bandicoot-NSAMETRIOLOGY-Tool** [download](https://github.com/pashok6798/Crash-Bandicoot-NSAMETRIOLOGY-Tool)


**For Linux users?** These tools are compatible with Windows, but they work pretty good with wine/mono, about quickbms it works, but there is also the source code available.

 
---


## Crash Bandicoot Trilogy (PS1)

The Crash Bandicoot Trilogy games are composed by ***.NSD, *.NSF** file how to get them?
If you have the **Game.cdz** you can convert it to Game.bin with psxfin or cdztool (PSX tool included in the emulator) and then to Game.iso with ccd2iso if you use Linux/Mac or with [these tools](https://helpdeskgeek.com/free-tools-review/how-to-convert-bin-to-iso/) if you use Windows.
When you have the iso file you can easily extract it and get the NSD/NSF files.

When you have the NSD/NSF files you can open them with the tool **CrashEdit** or **drnsf**, the former allows to edit, play/export the sound file, the texture etc. the latter, allows to open the nsd/nsf file and view the 3D models.
**Drnsf** don't export the 3D models, while the last version of CrashEdit should allows to export the scenery 3d model.

Another tool that export the 3D models is **[Crash-Bandicoot-2-Modelexport](https://github.com/warenhuis/Crash-Bandicoot-2-Modelexport)** but it depends on CrashEdit as you can see in [this video](https://www.youtube.com/watch?v=g7ByLSotvNo).

A simple tool (for developers mainly) that only "load" the nsf file in memory and start to work on them could be [crash-bandicoot-nsf](https://github.com/dehodson/crash-bandicoot-nsf), is a simple python script to read the nsf file, you can use it to study how this kind of programs works and maybe write a new one.

### Tools summary
- **psxfin**, **cdztool**, **ccd2iso**
- **CrashEdit** [download](https://github.com/ManDude/CrashEdit/tree/newgui)
- **Crash-Bandicoot-2-Modelexport** [download](https://github.com/warenhuis/Crash-Bandicoot-2-Modelexport) [reference](https://www.youtube.com/watch?v=g7ByLSotvNo)
- **drnsf** [download](https://github.com/cbhacks/drnsf) 
- **PSXCrashTrilogyEditor** [download](https://github.com/TFSThiagoBR98/PSXCrashTrilogyEditor) 
- **crash-bandicoot-nsf** [download](https://github.com/dehodson/crash-bandicoot-nsf) 

---
### Other
- **Crash 2 engine in C** [download](https://github.com/ughman/c2c)
