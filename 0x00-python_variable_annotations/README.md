# Python Type Annotations Project

## Learning Objectives

By the end of this project, you should be able to:

- Understand and explain type annotations in Python 3.
- Use type annotations to specify function signatures and variable types effectively.
- Explain the concept of duck typing in Python.
- Validate Python code using `mypy`.

## Requirements

### General

- **Editors**: You may use `vi`, `vim`, or `emacs` for your project.
- **Python Version**: All your files will be interpreted and compiled using Python 3.7 on Ubuntu 18.04 LTS.
- **File Format**: Ensure that all files end with a new line.
- **Shebang**: The first line of all your files should be exactly:
  ```bash
  #!/usr/bin/env python3
  ```
- **README**: A `README.md` file at the root of the project folder is mandatory. This README explains the purpose, objectives, and any other relevant information regarding the project.
- **Code Style**: Follow the `pycodestyle` style guide (version 2.5).
- **File Execution**: All files must be executable.
- **File Length**: The length of your files will be tested using the `wc` command.

### Documentation

- **Module Documentation**: All your Python modules must include documentation. To check the documentation, you can run:
  ```bash
  python3 -c 'print(__import__("my_module").__doc__)'
  ```
- **Class Documentation**: Every class you create should be documented. Use the following command to check class documentation:
  ```bash
  python3 -c 'print(__import__("my_module").MyClass.__doc__)'
  ```
- **Function Documentation**: All functions, whether inside or outside of a class, should have documentation. Validate function documentation with:
  ```bash
  python3 -c 'print(__import__("my_module").my_function.__doc__)'
  python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)'
  ```
- **Documentation Quality**: Documentation should be more than just a single word. It must be a meaningful sentence explaining the purpose of the module, class, or method, and its length will be verified.

## Type Annotations

### Function Signatures

You will learn how to use type annotations to explicitly declare the types of arguments a function accepts and the type of value it returns. Example:

```python
def add(a: int, b: int) -> int:
    """Returns the sum of two integers."""
    return a + b
```

### Duck Typing

Duck typing is a concept in Python where an object's suitability is determined by the presence of certain methods and properties, rather than the actual type of the object. You'll explore how this works in Python code, allowing flexibility in handling different object types.

### Mypy

You'll use `mypy`, a static type checker for Python, to validate type annotations in your code. It ensures your type hints are correct, making your code more robust and reducing runtime errors. Example:

```bash
mypy my_code.py
```

## Project Setup

1. Clone the repository:
   ```bash
   git clone <repository_url>
   ```

2. Navigate to the project folder:
   ```bash
   cd <project_folder>
   ```

3. Make your Python files executable:
   ```bash
   chmod +x *.py
   ```

4. Run `mypy` on your files to check for any type validation errors:
   ```bash
   mypy your_file.py
   ```

## Useful Commands

- **Check pycodestyle compliance**:
  ```bash
  pycodestyle your_file.py
  ```

- **Check file length**:
  ```bash
  wc your_file.py
  ```

## Conclusion

By completing this project, you will enhance your understanding of Python's type system, improve code reliability, and develop well-documented, type-safe Python code.
