About this allocator
-----------------
This is the Lockless Allocator, derived from http://locklessinc.com/

Original sources located in ./src/

Please, look at the terms of usage: http://locklessinc.com/products/

What I did
-----------------
Since original allocator was released under GPL-3, I slightly modified sources to make it buildable for both VS and GCC. It was tested with VS 2013 and GCC 4.8 (both Linux and Windows builds were tested and work fine). Now it is possible to build allocator with all modern compilers, including
* Clang >=3.4
* GCC >=4.8 (including MinGW)
* and VS 2013

Both x86 (32bit) and x86-64 (64bit) builds should work without any problems for all listed compilers, but I wasn't tested all these possible variants.

In addition, I added CMake support, so allocator builds smoothly in both Linux and Windows (no need for POSIX emulation/Automake anymore).

TODO
-----------------
I want to add Mac OS X and FreeBSD support, but I don't feel like I need this right now. Maybe in the future I'll do this.