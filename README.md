Dependencies
============

# Platforms
The dependency package for various platforms:

## Android
This subdirectory includes packed sources of all libraries that are not included
in stk-code/lib and that are necessary to compile SuperTuxKart for Android.

## Windows
This subdirectory includes all files necessary to compile SuperTuxKart
with Visual Studio 2013 (or later).

## Windows-MinGW
This subdirectory includes all files necessary to compile SuperTuxKart with GCC
or Clang compiler on Windows.

## Windows-MinGW 64bit
This subdirectory includes all files necessary to compile 64-bit version of
SuperTuxKart with GCC compiler on Windows.

# Common problems 
## Copy files content not the symbolic links
Because some files are symbolic linked between each other you would need to copy the content
instead of the symbolic link instead when wanting to export dependency packages.

On unix systems (Linux, Mac, BSD, or even bash on windows), run the following command:
```sh
cp --dereference --recursive <SOURCE> <DESTINATION>

# So for example
cp --dereference --recursive windows/ windows-distribute/
```
