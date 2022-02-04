## Problem

The following error is found, even though `from google.cloud import storage` is valid.

```
$ mypy .
src/a.py:1: error: Module "google.cloud" has no attribute "storage"
Found 1 error in 1 file (checked 2 source files)
```

Curiously, commenting out the `import google.cloud.billing` line in `b/__init__.py` makes the error go away.
