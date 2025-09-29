# Septerra Core: Legacy of the Creator - PSVita port

![Screenshot](https://raw.githubusercontent.com/isage/septerra-core-vita/master/sce_sys/pic0.png)

This port is based on [SR project](https://github.com/M-HT/SR)  
That means it's a [statically recompiled](https://en.wikipedia.org/wiki/Binary_translation) binary with specific parts re-implemented with posix/vita compatibility.


## Running

* Install [fdfix](https://github.com/TheOfficialFloW/FdFix)
* Instal latest vpk from [releases](https://github.com/isage/septerra-core-vita/releases)
* Copy data from your legally obtained copy of the game into `ux0:/data/septerra/`
* If you want stretched fullscreen: create file with the name `fullscreen` inside `ux0:/data/septerra/`

![Controls](https://raw.githubusercontent.com/isage/septerra-core-vita/master/sce_sys/manual/001.png)
![Controls2](https://raw.githubusercontent.com/isage/septerra-core-vita/master/sce_sys/manual/002.png)

## Building

Yeah, good luck.
But seriously:
1. install [libquicktime](https://github.com/isage/libquicktime-vita)
2. clone https://github.com/M-HT/SR and apply patch. copy sce_sys to `games/Septerra Core/SR-Septerra`
3. build llasm and copy somewhere in the PATH
4. build SRW with scons, copy SRW.exe to `SRW-games/Septerra Core/SRW`
5. copy your Septerra104.exe to same dir. run build-llasm.sh
6. copy Septerra.llasm, and seg*.llinc files into `games/Septerra Core/SR-Septerra/llasm`
7. run `scons device=vita-llasm`
that should produce both eboot.bin and sc.vpk

## Thanks

* [Northfear](https://github.com/Northfear) for sdl1 vita port.
* [SonicMastr](https://github.com/SonicMastr) and [GrapheneCt](https://github.com/GrapheneCt) for libime code.

## License

MIT, Copyright 2022 Ivan Epifanov.
