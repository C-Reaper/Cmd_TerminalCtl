# Project README

## Overview
This project is a simple C program that demonstrates the use of a terminal control library (`TerminalCtl`). The main function initializes and manipulates a terminal, setting its size, clearing it, changing its color, and then resetting it. 

## Features
- Terminal resizing.
- Terminal updating.
- Terminal clearing.
- Setting terminal text color.
- Resetting terminal settings.

## Project Structure
### Prerequisites
- C/C++ Compiler and Debugger (GCC, Clang)
- Make utility
- Standard development tools

## Build & Run
The project includes makefiles for building on Linux, Windows, Wine, and WebAssembly. Here are the steps to build and run the project:

### Linux
To build:
```sh
make -f Makefile.linux all
```

To execute:
```sh
make -f Makefile.linux exe
```

### Windows
To build:
```sh
make -f Makefile.windows all
```

To execute:
```sh
make -f Makefile.windows exe
```

### Wine (Linux Cross-Compile for Windows)
To build:
```sh
make -f Makefile.wine all
```

To debug:
```sh
make -f Makefile.wine debug
```

To execute:
```sh
make -f Makefile.wine exe
```

### WebAssembly (Emscripten)
To build:
```sh
make -f Makefile.web all
```

To run the output:
```sh
wasmtime ./build/Main.wasm
```

These makefiles allow for clean builds and execution across different platforms. The project does not require any specific libraries beyond what is standard with most C/C++ development environments.