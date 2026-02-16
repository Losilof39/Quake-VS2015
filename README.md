# How to compile with CMake
To compile the source code with cmake make sure to use an MSVC compiler and compile in x86 architecture. Place the assets in the same directory of `winquake.exe` to play the game.

## Windows
Run this command in the `x86 Native Tools Command Prompt for VS` prompt to build and compile in debug mode, all in one line:
```
cmake -DCMAKE_BUILD_TYPE:STRING=Debug -B build -G Ninja && cd build && ninja
```
You can choose whatever generator you like to use, this one uses Ninja for fast compile times. The C compiler is not specified in the CMakelist.txt.

**Have fun!**

# Original repo info below

## Quake-VS2015
Publication of the Visual Studio 2015 Build of Quake

Just a single note to make. Visual Studio 2015 will attempt to build in x64 mode by default, but we are set up to build in x86 mode (or Win32 for previous versions of Visual Studio).

At the top of the Visual Studio window, if you see x64 in a drop down box, change it to x86 or Win32, whichever your version uses. Then build, and everything will compile.

Finally, you need the Id1 folder from a legitimate version of Quake (or shareware, or a mod if you have a mod that uses an unmodified Quake engine). The easiest thing to do is just buy Quake on Steam.

Goto my YouTube channel at http://youtube.com/philipbuuck or http://handmadequake.org for more information on the Handmade Quake project.

Happy hunting!
Philip Buuck
