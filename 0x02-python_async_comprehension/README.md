Python Async Comprehension Project

## Overview

This project focuses on understanding and implementing asynchronous generators and comprehensions in Python. The tasks guide you through creating an asynchronous generator, utilizing async comprehensions, and measuring the runtime for parallel comprehensions.

**Author:** Emmanuel Turlay, Staff Software Engineer at Cruise

**Weight:** 1

## Project Timeline

- **Start Date:** Jan 16, 2024, 6:00 AM
- **End Date:** Jan 17, 2024, 6:00 AM
- **Checker Release:** Jan 16, 2024, 12:00 PM
- **Auto Review:** At the deadline

## Requirements

### General

- **Allowed Editors:** vi, vim, emacs
- **Environment:** Ubuntu 18.04 LTS, Python 3.7
- **File Endings:** All files should end with a new line
- **Shebang Line:** The first line of all files should be exactly `#!/usr/bin/env python3`
- **Documentation:** README.md file at the root is mandatory
- **Code Style:** Pycodestyle style (version 2.5.x)
- **File Length:** The length of your files will be tested using `wc`
- **Module Documentation:** `python3 -c 'print(__import__("my_module").__doc__)'`
- **Function Documentation:** `python3 -c 'print(__import__("my_module").my_function.__doc__)'`
- **Function and Coroutine Annotations:** All functions and coroutines must be type-annotated

### Tasks

#### Task 0: Async Generator

- **Objective:** Write a coroutine (`async_generator`) to loop 10 times, asynchronously waiting 1 second, then yielding a random number between 0 and 10.

- **Example:**
  - Input: `async_generator()`
  - Output: `[4.403136952967102, 6.9092712604587465, ...]`

#### Task 1: Async Comprehensions

- **Objective:** Write a coroutine (`async_comprehension`) to collect 10 random numbers using async comprehensions over `async_generator`.

- **Example:**
  - Input: `async_comprehension()`
  - Output: `[9.861842105071727, 8.572355293354995, ...]`

#### Task 2: Run time for four parallel comprehensions

- **Objective:** Write a `measure_runtime` coroutine to execute `async_comprehension` four times in parallel using `asyncio.gather`. Measure the total runtime.

- **Example:**
  - Input: `measure_runtime()`
  - Output: `10.021936893463135`

## Usage

### Running the Test Scripts

Use the provided test scripts (e.g., `0-main.py`, `1-main.py`, `2-main.py`) to check the functionality of your implementations.

```bash
./0-main.py
./1-main.py
./2-main.py
```

### Code Integration

Integrate the provided test scripts into your solution for validation.

## Conclusion

This project aims to enhance your understanding of asynchronous generators and comprehensions in Python. Follow the tasks sequentially, ensuring proper documentation, adherence to coding standards, and correct implementation of asynchronous concepts.

---
