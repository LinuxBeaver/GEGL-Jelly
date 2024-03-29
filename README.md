
## GEGL Jelly a Gimp Plugin that covers things in goo. 

This filter requires
https://github.com/LinuxBeaver/GEGL-Custom-Bevel to work.

People who wish to compile will have to go here to compile custom bevel.
It will not work proper at all without it. People who uses binaries can find
the binary of custom bevel included.


![image preview](jelly.png )



## OS specific location to put GEGL Filter binaries 

Windows
C:\Users\USERNAME\AppData\Local\gegl-0.4\plug-ins
 
 Linux 
 /home/(USERNAME)/.local/share/gegl-0.4/plug-ins
 
 Linux (Flatpak)
 /home/(USERNAME)/.var/app/org.gimp.GIMP/data/gegl-0.4/plug-ins



## Compiling and Installing

### Linux

To compile and install you will need the GEGL header files (`libgegl-dev` on
Debian based distributions or `gegl` on Arch Linux) and meson (`meson` on
most distributions).

```bash
meson setup --buildtype=release build
ninja -C build

```

If you have an older version of gegl you may need to copy to `~/.local/share/gegl-0.3/plug-ins`
instead (on Ubuntu 18.04 for example).



### Windows

The easiest way to compile this project on Windows is by using msys2.  Download
and install it from here: https://www.msys2.org/

Open a msys2 terminal with `C:\msys64\mingw64.exe`.  Run the following to
install required build dependencies:

```bash
pacman --noconfirm -S base-devel mingw-w64-x86_64-toolchain mingw-w64-x86_64-meson mingw-w64-x86_64-gegl
```

Then build the same way you would on Linux:

```bash
meson setup --buildtype=release build
ninja -C build
```

## more image previews just to show off how based the plugin is.

![image](https://github.com/LinuxBeaver/GEGL-Jelly/assets/78667207/d29d64f8-1120-4b5d-b0c1-70ea9f610f84)
meme reference https://www.youtube.com/watch?v=ze4NQTXvxYc
![image](https://github.com/LinuxBeaver/GEGL-Jelly/assets/78667207/7c18b077-aba9-49f5-bd07-700e51c277d5)




