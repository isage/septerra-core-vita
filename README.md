# Septerra Core: Legacy of the Creator - PSVita port

![Screenshot](https://raw.githubusercontent.com/isage/septerra-core-vita/master/sce_sys/pic0.png)

This port is based on [SR project](https://github.com/M-HT/SR)  
That means it's a [statically recompiled](https://en.wikipedia.org/wiki/Binary_translation) binary with specific parts re-implemented with posix/vita compatibility.


## Running

* Install [fdfix](https://github.com/TheOfficialFloW/FdFix)
* Instal latest vpk from [releases](https://github.com/isage/septerra-core-vita/releases)
* Copy data from your legally obtained GOG copy of the game into `ux0:/data/septerra/`
* Note:  
  if you're using original non-GOG release ( or any other that don't have m1.avi-m9.avi, etc.)
  * install quicktime 4 (comes with original release)
  * download [unofficial Timesplip patch](http://timeslip.users.sourceforge.net/current/sc_patch.exe) and run it
  * copy .avi files, but don't copy .DB files with same name

![Controls](https://raw.githubusercontent.com/isage/septerra-core-vita/master/sce_sys/manual/001.png)

## Building

Yeah, good luck.

## Thanks

* [Northfear](https://github.com/Northfear) for sdl1 vita port.
* [SonicMastr](https://github.com/SonicMastr) and [GrapheneCt](https://github.com/GrapheneCt) for libime code.

## License

MIT, Copyright 2022 Ivan Epifanov.