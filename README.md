BASH.helpers
============

A collection of useful BASH scripts and functions.

  [go](#go)

## License

All scripts and functions contained in this collection are subject to the

 MIT License (MIT)

 Copyright (c) 2014 Mathias Gelhausen <devel@tisie.de>

 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files
 (the "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
 the following conditions:

 The above copyright notice and this permission notice shall be
 included in all copies or substantial portions of the Software.

 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
 OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
 CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.


## go

"go" is a bash function that create and manage directory shortcuts.

### Installation

source the file "functions/go.func" 

```
. functions/go.func
source functions/go.func
```

For permanent availability include the above statement in your .bashrc

### Usage

```
  go                                     # List all defined shortcuts

  go + demo                              # adds a shortcut to the current directory
                                         # with the name "demo"

  go + test /some/very/often/used/dir    # adds a shortcut to the given directory
                                         # with the shortcut "test"

  go test                                # jumps to the directory with the shortcut name "test"
  go te                                  # jumps also to test, because partially typed
                                         # names are resolved using the first match in list

  go demo                                # jumps to the directory defined under "demo"

  go - test				 # deletes shortcut "test"

```

