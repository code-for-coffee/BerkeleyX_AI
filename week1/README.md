# Python

* `brew install python` (or some other installation method)
* To open the Python REPL: `python`
* String method use:
  * `"artificial".upper() # ARTIFICIAL`
  * `"artificial".lower() #'artificial'`
* Do not need to declare variables before defining them.
* Variable declaration:
  * `msg = "hello, friends"`
  * `len(msg.upper()) #14`

## Methods
* To see what methods Python provides for a datatype, use the `dir` and help commands...
* `ai = 'robot?'`
* `dir(ai)` returns:
* `['__add__', '__class__', '__contains__', '__delattr__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__getitem__', '__getnewargs__', '__getslice__', '__gt__', '__hash__', '__init__', '__le__', '__len__', '__lt__', '__mod__', '__mul__', '__ne__', '__new__', '__reduce__', '__reduce_ex__', '__repr__', '__rmod__', '__rmul__', '__setattr__', '__sizeof__', '__str__', '__subclasshook__', '_formatter_field_name_split', '_formatter_parser', 'capitalize', 'center', 'count', 'decode', 'encode', 'endswith', 'expandtabs', 'find', 'format', 'index', 'isalnum', 'isalpha', 'isdigit', 'islower', 'isspace', 'istitle', 'isupper', 'join', 'ljust', 'lower', 'lstrip', 'partition', 'replace', 'rfind', 'rindex', 'rjust', 'rpartition', 'rsplit', 'rstrip', 'split', 'splitlines', 'startswith', 'strip', 'swapcase', 'title', 'translate', 'upper', 'zfill']`
* Using `.split()`:
* `ai.split('?') # ['robot', '']`

## help()
* You can open the API documentation for Python directly in the REPL. There is a built in `help()` command where you can enter in a method for documentation. For example, `help(ai.find)` returns:

```python
Help on built-in function find:

find(...)
    S.find(sub [,start [,end]]) -> int

    Return the lowest index in S where substring sub is found,
    such that sub is contained within S[start:end].  Optional
    arguments start and end are interpreted as in slice notation.

    Return -1 on failure.
```

Note this is open in a terminal text editor. You may need to close the documentation by pressing `:` + `q` or `ctrl` + `x`.

## Lists

* Lists are like arrays, but with fundamental differences:
* They are a data type in Python.
* `fruits = ['apple','orange','pear','banana']`
* `otherFruits = ['kiwi','strawberry']`
* You can concatenate lists together!
* `fruits + otherFruits #['apple', 'orange', 'pear', 'banana', 'kiwi', 'strawberry']`
* Python also allows negative-indexing from the back of the list. For instance, `fruits[-1]` will access the last element `'banana'`
* List Methods:
  - 'append',
  - 'count',
  - 'extend',
  - 'index',
  - 'insert',
  - 'pop',
  - 'remove',
  - 'reverse',
  - 'sort'
* Start/Stop Syntax
  * `fruits[start:stop]`
  * Select a starting element : ending element
  * Get all the things between!
  * `fruits[1:2] #['orange']`
  * Start at 2:
  * `fruits[2:] #['pear', 'banana']`
  * Stop at :2
  * `fruits[:2] #['apple', 'orange']`
* The items stored in lists can be any Python data type.
