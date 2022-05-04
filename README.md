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
## License
Copyright 2017-2022 The Pixellizer Group

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.