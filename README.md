# CMake tutorial
CMake templates and tutorials for starting C++ projects from scratch

## Getting started on Linux

### Prerequisites
```bash
$ sudo apt install build-essential make cmake
```

### Starting the project
```bash
$ git clone git@github.com:srbdev/cmake_tutorial.git
$ cd cmake_tutorial
$ mkdir build
$ cd build
$ cmake ..
$ make
$ ./tutorial
test!
```

## Getting started on Mac

## Getting started on Windows

### Prerequisites
You will need to install [Visual Studio Community 2019](https://visualstudio.microsoft.com/vs/) and [CMake](https://cmake.org/download/).

### Starting the project
```powershell
> git clone git@github.com:srbdev/cmake_tutorial.git
> cd cmake_tutorial
> mkdir build
> cd build
> cmake -G "Visual Studio 16" ..
```

Using File Explorer, navigate to the build directory and double-click on the file `Tutorial.sln`.
It will open Visual Studio for you with Tutorial project setup. In the Solution Explorer, right click
on the `ALL_BUILD` project and select `Build`.

```powershell
> cd Debug
> .\tutorial.exe
test!
```
