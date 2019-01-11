# ZLint

Source code linting utilities for C++ and Python: [cpplint.py](cpplint.py), [pylint.py](pylint.py).

Cyclomatic complexity analyzer (C++ source): [hfcca.py](hfcca.py).
> [what is cyclomatic complexity?](https://en.wikipedia.org/wiki/Cyclomatic_complexity), [an example of Go project](https://goreportcard.com/report/github.com/pingcap/tidb)

### Note

Except [hfcca.py](hfcca.py), files here are copied from the [Chromium Project](https://www.chromium.org/)'s [depot_tools](https://chromium.googlesource.com/chromium/tools/depot_tools.git).

[hfcca.py](hfcca.py) is a very early fork of [Linzard](https://github.com/terryyin/lizard).

### Help message
```
./cpplint.py --help
```
gives [C++ linter help](cpplint.py.help.md).

```
./pylint.py --help
```
gives [Python linter help](pylint.py.help.md).

```
./hfcca.py --help
```
gives [CCN counter help](hfcca.py.help.md).

### Prerequisites
Python2.7, no external packages required.

Python3 might work, no errors detected.

### License
[hfcca.py](hfcca.py) has its own copyright license, see inside.

Except [hfcca.py](hfcca.py): unless otherwise noted, use of the source code are governed by Chromium's BSD-style [license](LICENSE.chromium).

###### EOF
