# hfcca.py

```
Usage: hfcca.py [options] [PATH or FILE] [PATH] ... 

A simple code complexity source file counter ignoring C/C++ header files. It
can deal with C/C++/Obj-C & TNSDL code. It counts the NLOC (lines of code
without comments), CCN (cyclomatic complexity number) and token count of
functions. It requires python2.6 or above (early versions are not verified).

Options:
  -h, --help            show this help message and exit
  -v, --verbose         Output in verbose mode (long function name)
  -C CCN, --CCN=CCN     Threshold for cyclomatic complexity number warning.
                        _functions with CCN bigger than this number will be
                        shown in warning
  -w, --warnings_only   Show warnings only
  -i NUMBER, --ignore_warnings=NUMBER
                        If the number of warnings is equal or less than the
                        number, the tool will exit normally, otherwize it will
                        generate error. Useful in makefile when improving
                        legacy code.
  -x EXCLUDE, --exclude=EXCLUDE
                        Exclude data files that match this regular expression.
                        Multiple regular expressions can be specified.
  -X, --xml             Generate XML in cppncss style instead of the normal
                        tabular output. Useful to generate report in Hudson
                        server
  -p, --preprocess      Use preprocessor, always ignore the #else branch. By
                        default, hfcca just ignore any preprocessor statement.
  -a ARGUMENTS, --arguments=ARGUMENTS
                        Limit for number of parameters
  -P, --no_preprocessor_count
                        By default, a #if will also increase the complexity.
                        Adding this option to ignore them
  -t WORKING_THREADS, --working_threads=WORKING_THREADS
                        number of working threads. The default value is 1.
```

###### EOF
