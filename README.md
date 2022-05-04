# 3gxtool
An utility to create *3GX* game plugins from *ELF* and *plginfo* files.

## Installing
You can place this tool in any folder in your path to be able to build *3GX* plugins with their provided *Makefiles*
## Usage
```
3gxtool [OPTION...] <input.bin> <settings.plgInfo> <output.3gx>
Available options:
    -d, --discard-symbols: Don't include the symbols in the file
    -s, --silent: Don't display the text (except errors)
    -e, --enclib: Encryption shared library
    -h, --help: Print help
```
## Building
You need *cmake* in order to build this tool. If you are building in windows, you need the GNU C++ compiler (for example the one provided by MSYS or MINGW).

### Windows
Alternatively in the 3rd line, use "MINGW Makefiles" or any other option that uses the GNU C++ compiler.
```
mkdir build
cd build
cmake .. -G "MSYS Makefiles"
cmake --build .
```

### Linux
```
mkdir build
cd build
cmake ..
cmake --build .
```