# Mini Compiler in C++

A modular compiler implementation written in C++ to explore compiler architecture, intermediate representations, optimization techniques, and low-level program translation.

## Overview

This project implements a miniature compiler with a focus on understanding how source code is processed through different stages of a compilation pipeline. It is designed with a modular architecture, testable components, and an emphasis on correctness and maintainability.

The project explores core compiler concepts, including lexical analysis, parsing, intermediate representation (IR), optimization, and code generation.

## Features

* **Lexical Analysis:** Tokenizes source input into meaningful language elements.
* **Parsing:** Processes tokens according to the language grammar.
* **Intermediate Representation:** Represents programs in a form suitable for analysis and transformation.
* **Compiler Optimizations:** Implements optimization passes such as constant folding and dead code elimination.
* **Modular Architecture:** Separates compiler components into maintainable C++ modules.
* **Automated Testing:** Uses a test suite to validate compiler behavior and optimization correctness.
* **Build and Verification:** Supports a repeatable build and testing workflow.

## Architecture

The compiler is organized around a pipeline of processing stages:

```
Source Code
    |
    v
Lexical Analysis
    |
    v
Parsing
    |
    v
Intermediate Representation
    |
    v
Optimization Passes
    |
    v
Code Generation
    |
    v
Output
```

## Optimization

The optimization component is designed around independently testable passes. These include:

* **Constant Folding:** Evaluates constant expressions at compile time.
* **Dead Code Elimination:** Removes code that does not contribute to program results.

The modular design makes it possible to test optimization passes individually and verify their behavior against expected results.

## Technology Stack

* **Language:** C++
* **Build System:** CMake
* **Testing:** Automated unit and regression tests
* **Development Environment:** Visual Studio Code

## Building and Testing

The project uses CMake for configuration and building.

```
cmake -S . -B build
cmake --build build
```

Run the project's test suite using the test commands or verification scripts provided in the repository.

On Windows, use the supplied Windows verification script if available.

## Project Goals

* Understand the internal stages of a compiler.
* Apply C++ to a systems programming project.
* Explore intermediate representations and compiler optimization.
* Build reliable, independently testable components.
* Strengthen debugging, testing, and software design skills.

## Future Improvements

* Expand the supported language syntax.
* Introduce additional optimization passes.
* Improve diagnostics and error reporting.
* Extend code generation and runtime validation.
* Add benchmarks for evaluating optimization effectiveness.
