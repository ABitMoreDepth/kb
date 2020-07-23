# Python Imports

If you ship a library/application with no source files & a collection of
bytecode files, it turns out you can mess with things by adding a
`__init__.py` file somewhere in the byte-compiled shipped library code. When
[[Python]] comes to import what you expect to be the byte-compiled code, it
will actually default to the source file first.

Ref: [Python Imports](https://docs.python.org/3/reference/import.html)

Obvious import candidates:
- *.py
- *.pyc

Less obvious ones:
- *.pyo
- *.pyd

These latter two are related to bytecode thats been optimised, and python
windows DLL files, specific to the windows platform.

Can override import hooks etc. to customise import behaviour. This I believe
is what [[pyinstaller]] does by default.

Is there anything that [[pyinstaller]] can import?

[Core module loading interface](https://docs.python.org/3/library/importlib.html#importlib.abc.Loader.exec_module)

Python will check byte-code (pyc) against the source python file if
available, so the (.py) file will always be preferred to the bytecode file.

