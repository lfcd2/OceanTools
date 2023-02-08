# OceanTools
Tools for ocean carbon practical

## Compile working.py for distributions:

1. `pyenv local 3.8.10` (update version to match Google Colab python version.)
2. `python -m compileall ./tools` which creates a `__pycache__` folder with compiled python files.
3. Copy `working.cpython-38.pyc` to `working.py` in the `tools` folder to make compiled funcitons accessible to Google Colab.
4. Commit these to master, but keep `working.py` in `dev`.