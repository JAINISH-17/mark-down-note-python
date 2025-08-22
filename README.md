# Python PVM & Garbage Collector

## Python Virtual Machine (PVM)

- The Python Virtual Machine (PVM) is the runtime engine of Python.
- It executes the compiled bytecode (.pyc files) produced by the Python interpreter.
- PVM is responsible for interpreting instructions, managing memory, and handling dynamic typing.
- The process:
  1. Python source code (.py) is converted into bytecode.
  2. Bytecode is executed by the PVM.
- The PVM is platform-dependent and abstracts hardware details, allowing Python code to run on various systems.

## Python Garbage Collector

- Python manages memory automatically using a built-in garbage collector.
- Primary mechanism: **Reference Counting**
  - Each object keeps track of how many references point to it.
  - When the count drops to zero, the object is deleted.
- **Cyclic Garbage Collection**
  - Handles reference cycles (objects referencing each other, forming a cycle).
  - The `gc` module can be used to control and interact with the garbage collector.
  - Example usage:
    ```python
    import gc
    References
Python Documentation: Memory Management
Python gc module

    # Force a garbage collection
    gc.collect()
    ```
- Garbage collection is essential to prevent memory leaks and optimize resource usage.

## Summary# mark-down-note-python
