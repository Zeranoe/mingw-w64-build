# mingw-w64-build
mingw-w64-build is a Bash script to build a [MinGW-w64](https://mingw-w64.org)
cross compiler for i686 (Win32) and x86_64 (Win64). It will build a fully static
toolchain that can compile Windows executables that don't depend on any GCC dll
files.

## Default Branches
* [MinGW-w64](https://mingw-w64.org) master
* [Binutils](https://www.gnu.org/software/binutils/) binutils-2_45-branch
* [GCC](https://gcc.gnu.org/) releases/gcc-15

## Default Prefix
`$HOME/.zeranoe/mingw-w64/i686` and `$HOME/.zeranoe/mingw-w64/x86_64` are the
default install locations, but this location can be modified with the `--prefix`
option. To ensure the new compilers are available system-wide, add
`$HOME/.zeranoe/mingw-w64/<arch>/bin` to the `$PATH`.

## Platforms
mingw-w64-build should run on Ubuntu, Cygwin, macOS (with Homebrew), and other
Bash based shells.

## Usage
See `mingw-w64-build --help` for all build options.

## License
mingw-w64-build is licensed under the GNU GPL 3.0 or later. A copy of the
license can be found in the LICENSE file.
