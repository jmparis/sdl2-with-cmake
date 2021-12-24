# sdl2-with-cmake
A simple example that combines SDL2 application with cmake toolchain.
This Git project use another Git submodule specific for `cmake`.
This submodule help to find and resolve all required references for SDL2 libraries.

## Usage
``` Shell
sdl2-with-cmake
❯ mkdir build; cd build

sdl2-with-cmake/build
❯ cmake ..
-- The C compiler identification is GNU 11.1.0
-- The CXX compiler identification is GNU 11.1.0
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /usr/sbin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /usr/sbin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Found SDL2: /usr/lib/libSDL2.so (found version "2.0.18")
-- Found SDL2_net: /usr/lib/libSDL2_net.so (found version "2.0.1")
-- Found SDL2_mixer: /usr/lib/libSDL2_mixer.so (found version "2.0.4")
-- Found SDL2_image: /usr/lib/libSDL2_image.so (found version "2.0.5")
-- Found SDL2_gfx: /usr/lib/libSDL2_gfx.so (found version "1.0.4")
-- Found SDL2_ttf: /usr/lib/libSDL2_ttf.so (found version "2.0.15")
-- Configuring done
-- Generating done
-- Build files have been written to: /home/jean-michel/Repos/sdl2-with-cmake/build

sdl2-with-cmake/build
❯ make
[ 50%] Building C object CMakeFiles/simple-window.dir/src/main.c.o
[100%] Linking C executable simple-window
[100%] Built target simple-window
```