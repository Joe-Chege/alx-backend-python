## README: Python Variable Annotations Project

Welcome to the Python Variable Annotations Project! This project focuses on enhancing your understanding of Python 3 type annotations. Follow the steps below to complete the tasks successfully.

### Project Overview

- **Title:** Python Variable Annotations
- **Domain:** Python
- **Author:** Emmanuel Turlay, Staff Software Engineer at Cruise
- **Weight:** 1
- **Project Start:** Jan 11, 2024 6:00 AM
- **Project End:** Jan 12, 2024 6:00 AM
- **Auto Review:** Scheduled at the deadline

### Learning Objectives

By the end of this project, you should be able to:

- Explain type annotations in Python 3.
- Use type annotations to specify function signatures and variable types.
- Understand duck typing principles.
- Validate your code with MyPy.

### Requirements

- **Editors:** Allowed editors include vi, vim, and emacs.
- **Python Version:** All files will be interpreted/compiled on Ubuntu 18.04 LTS using Python 3.7.
- **File Endings:** Ensure all your files end with a new line.
- **Shebang Line:** The first line of all your files should be `#!/usr/bin/env python3`.
- **README.md:** A mandatory README.md file at the root of the project folder.
- **Code Documentation:** Your code should be well-documented.
- **PEP 8 Style:** Follow PEP 8 style (version 2.5).
- **Executable Files:** All your files must be executable.
- **File Length:** The length of your files will be tested using `wc`.
- **Module Documentation:** All your modules should have documentation (`python3 -c 'print(__import__("my_module").__doc__)'`).
- **Class Documentation:** All your classes should have documentation (`python3 -c 'print(__import__("my_module").MyClass.__doc__)'`).
- **Function Documentation:** All your functions should have documentation (`python3 -c 'print(__import__("my_module").my_function.__doc__)'` and `python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)'`).

### Task Instructions

#### Task 0: Basic Annotations - Add

Write a type-annotated function `add` that takes two float arguments and returns their sum as a float.

```bash
# Command to test
./0-main.py
```

#### Task 1: Basic Annotations - Concat

Write a type-annotated function `concat` that takes two string arguments and returns a concatenated string.

```bash
# Command to test
./1-main.py
```

#### Task 2: Basic Annotations - Floor

Write a type-annotated function `floor` that takes a float argument and returns its floor value.

```bash
# Command to test
./2-main.py
```

#### Task 3: Basic Annotations - To String

Write a type-annotated function `to_str` that takes a float argument and returns its string representation.

```bash
# Command to test
./3-main.py
```

#### Task 4: Define Variables

Define and annotate specified variables with given values.

```bash
# Command to test
./4-main.py
```

#### Task 5: Complex Types - List of Floats

Write a type-annotated function `sum_list` that takes a list of floats and returns their sum.

```bash
# Command to test
./5-main.py
```

#### Task 6: Complex Types - Mixed List

Write a type-annotated function `sum_mixed_list` that takes a list of integers and floats and returns their sum.

```bash
# Command to test
./6-main.py
```

#### Task 7: Complex Types - String and Int/Float to Tuple

Write a type-annotated function `to_kv` that takes a string and an int or float, returning a tuple.

```bash
# Command to test
./7-main.py
```

#### Task 8: Complex Types - Functions

Write a type-annotated function `make_multiplier` that takes a float and returns a function to multiply a float by the given multiplier.

```bash
# Command to test
./8-main.py
```

#### Task 9: Let's Duck Type an Iterable Object

Annotate the parameters and return values of the `element_length` function.

```bash
# Command to test
./9-main.py
```

#### Task 10: Duck Typing - First Element of a Sequence

Augment the `safe_first_element` function with correct duck-typed annotations.

```bash
# Command to test
./100-main.py
```

#### Task 11: More Involved Type Annotations

Add type annotations to the `safely_get_value` function using TypeVar.

```bash
# Command to test
./101-main.py
```

#### Task 12: Type Checking

Use MyPy to validate and apply necessary changes to the `zoom_array` function.

```bash
# MyPy Command
mypy 102-type_checking.py

# Command to test
./102-main.py
```

### Conclusion

This project provides a comprehensive overview of Python variable annotations. Follow the steps and commands to complete each task successfully. Happy coding!