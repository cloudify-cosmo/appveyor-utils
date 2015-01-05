appveyor-utils
==============

[Appveyor](http://www.appveyor.com/) bootstrap scripts for unit testing Python projects under Windows.

Based on the excellent example of [Olivier Grisel](https://github.com/ogrisel/python-appveyor-demo).


How to use this?
================

1. Follow Appveyor's [insturctions](http://www.appveyor.com/docs) and add project
2. Copy `appveyor.yml` from the root of this repository into the root folder of your repository
3. Edit `tox.ini` (if needed)
4. Run new build from Appveyor control panel


Tox
====

Create new tox `testenv`:

```ini
[testenv:pywin]
deps =
    ...
basepython = {env:PYTHON}\python.exe
```