Android GNSS Logger to RINEX converter
======================================


This repository contains a Python script that converts logs from Google's GNSS
measurement tools to RINEX.  It was originally forked from 
https://github.com/rokubun/android_rinex but has been substantially modified.

See gnslogger_to_rnx.py for sample usage and a list of command line options.

`rtklibexplorer`'s fork has been modified in `plutonheaven`'s fork to use the code as a package in another project.

To do so, add the following line to your projects `pyproject.toml`:
```
dependencies = [
   ...
   "android_rinex==0.1.0",
]

[tool.uv.sources]
android_rinex = { git = "https://github.com/plutonheaven/android_rinex", branch = "master" }
```