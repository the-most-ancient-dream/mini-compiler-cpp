# Assembler and Linker in C++

A systems programming project that explores how assembly instructions are translated into machine-code representations and how separately assembled object files are combined into a linked program.

## Overview

This project implements an assembler and linker for a custom instruction set using C++. The assembler translates supported assembly instructions into machine-code representations, while the linker resolves symbols and combines object files into a unified output.

The project focuses on instruction encoding, symbol-table management, label resolution, relocation, and the organization of low-level program components.

## Features

* **Instruction Encoding:** Converts supported assembly instructions into machine-code representations.
* **Symbol Tables:** Records labels and symbols with their associated addresses.
* **Label Resolution:** Resolves symbolic references to instruction or data locations.
* **Object Files:** Represents assembled code and the information required for linking.
* **Relocation:** Adjusts address-dependent references when code or data locations change.
* **Multi-File Linking:** Combines multiple object files and resolves cross-file symbol references.
* **Automated Testing:** Validates instruction encoding, symbol resolution, relocation, and linking behavior.

## Architecture

```
Assembly Source Files
         |
         v
      Assembler
         |
         v
   Object Files
         |
         v
       Linker
         |
         v
  Symbol Resolution
         |
         v
      Relocation
         |
         v
    Linked Output
```

## Core Concepts

### Assembler

The assembler processes supported instructions and converts them into machine-code representations. It maintains symbol information and resolves labels according to the custom instruction-set design.

### Symbol Tables

Symbol tables associate labels with addresses or other symbol metadata. They support references within a source file and references that must be resolved during linking.

### Relocation

Relocation updates address-dependent references when code or data is placed at different locations in the final output. This allows separately assembled components to be combined correctly.

### Linker

The linker combines object files, resolves references between separately defined symbols, and applies relocation information to produce the final linked output.

## Technology Stack

* **Language:** C++
* **Domain:** Systems Programming
* **Core Topics:** Instruction encoding, symbol tables, relocation, object files, linking
* **Testing:** Automated test cases

## Building and Testing

Build the project using the build system configured in the repository.

If the project uses CMake, run:

```
cmake -S . -B build
cmake --build build
```

Run the available test suite to validate instruction encoding, label resolution, relocation, and multi-file linking.

## Project Goals

* Understand the relationship between assembly language and machine code.
* Explore symbol resolution and relocation at a low level.
* Implement modular assembler and linker components in C++.
* Develop reliable test cases for systems software.
* Strengthen debugging and software design skills.

## Future Improvements

* Expand the custom instruction set.
* Add more addressing modes and instruction formats.
* Improve error reporting for invalid instructions and undefined symbols.
* Add support for additional object-file metadata.
* Develop test programs that exercise complex cross-file references.

## License

Choose a license before distributing or accepting contributions to this project.
