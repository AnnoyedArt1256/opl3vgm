# opl3vgm: a simple OPL1/2/3 VGM player in C with SDL2

This project plays VGM files through OPL emulators (emu8950 and Nuked-OPL3 more specifically).

### What you need to use the binary
* SDL2 and SDL2_mixer Binaries

### What you need to compile
* a C compiler (duh)
* SDL2 and SDL2_mixer compiler files

### Notes
* OPL3 4OP modes are not visualized correctly.
* .vgz files are not supported.
* Dual-chip .vgm files and .vgm files which include chips other than OPL1/2/3 are not supported.
* The visualizer is only for educational and/or entertainment purposes only.
* I edited Nuked-OPL3's code so that it allows custom clock speeds
* I fixed a lot of bugs that were in opl3vgm_cli

### How to Compile
You can use this one-liner to compile this program:
```
gcc main.c opl3.c emu8950.c emuadpcm.c <SDL2 compiler flags> -o opl3vgm
```
then you can run the program by importing a VGM file as an argument:
```
./opl3vgm Drax_-_Bus.vgm
```
libraries used:
<br>
![emu8950](https://github.com/digital-sound-antiques/emu8950)
<br>
![Nuked-OPL3](https://github.com/nukeykt/Nuked-OPL3)

2022 AArt1256
