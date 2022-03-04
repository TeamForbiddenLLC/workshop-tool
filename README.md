
# Warfork Steam Workshop Upload Tool
A desktop tool for uploading Warfork content to the Steam Workshop. Shipped with Warfork (FVI Launcher) on Steam.

[![Build Status][travis-badge]][travis-url]
[![Build Status][appveyor-badge]][appveyor-url]

https://warfork.com/

[travis-badge]: https://travis-ci.com/TeamForbiddenLLC/warfork-steam-workshop.svg?branch=master
[travis-url]: https://travis-ci.com/TeamForbiddenLLC/warfork-steam-workshop/
[appveyor-badge]: https://ci.appveyor.com/api/projects/status/663w96wel5t5f7xu/branch/master?svg=true
[appveyor-url]: https://ci.appveyor.com/project/Warfork/warfork-steam-workshop

## Building

#### Dependencies:
```
cmake 3.0 or newer
C++14 compiler
Qt5.6 or newer (Any version of Qt5 *should* work though)
Steamworks SDK (see steamworks/readme.txt)
```

To build and run on Linux/OSX: 

```
$ cd warfork-steam-workshop
$ cmake -H. -Bbuild
$ cmake --build build --config release -- -j4
...
$ cd build
$ ./warfork-workshop-tool
```  

On Windows:

```
_ cmake -G "Visual Studio 15 Win64" -H. -Bbuild
_ cmake --build build --config release
...
_ cd build/Release
_ warfork-workshop-tool
```
