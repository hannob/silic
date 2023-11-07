# silic
silic - simple link checker written in python

# what?

Dissatisfied with all the link checkers I could find I wrote my own.

It takes an URL, will recursively try to get more HTML pages from the same hostname up
to a depth of 3 (configurable via command line) and will check all src and href
references for errors.

# usage

```
usage: silic [-h] [-m MAXDEPTH] [-q] [-d] url

positional arguments:
  url                   urls to scan

optional arguments:
  -h, --help            show this help message and exit
  -m MAXDEPTH, --maxdepth MAXDEPTH
                        Maximum depth on start domain
  -q, --quiet           Only output findings
  -d, --debug           Show detailed debugging info

```

# contributions

If you want to write pull requests please stick to the coding style.

```
pycodestyle silic  --ignore=E501,W503
pyflakes silic
```

should output no warnings.

# copyright

This code is licensed as 0BSD.
