Argpar
======

A simple argument parser.

Usage
-----

```python
import argpar
import copy
import sys
opts = {"o": None, "g": "foo", "w": None}
flags = ["t", "u"]
posarg = {"path": "/home"}
argpar.parse(opts, copy.copy(sys.argv), flags, posarg)
```

Vaules in `opts` and `posarg` dictionaries are default values.

Will automaticaly print help message if a `h` flag is found and exit.

We recomend copying `sys.argv`, as arguments get removed during parsing.