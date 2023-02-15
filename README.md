# OceanTools
Tools for ocean carbon practical

## Compile working.py for distributions:

Open a google colab notebook and run:

```
!rm -R OceanTools
!git clone https://github.com/Quantitative-Environmental-Science/OceanTools.git;cd OceanTools;git checkout dev
!cd OceanTools;python -m compileall ./tools
```

Followed by:

```python
from google.colab import files
from glob import glob

f = glob('OceanTools/tools/__pycache__/working*')
files.download(f[0])
```

This will download a file `working.cpython-XX.pyc`, which should be renamed to `working.py` and placed in `OceanTools/tools/working.py` on the `main` branch.