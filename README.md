# PyBlender
This is info library for Python Scripts in Blender. I will collect here usefull tipps and
examples of scripts to deal with blender >2.8.

**Where is my Console?**
To see errors and hints have a look at the system console. To do This
*Window* > *Toggle System Console*

## Include Python modules (libraries)
How to include your own libraries? You have to change the Python SystemPath (i call it).
```python
import sys
sys.exec_prefix

import os
rootPath = os.path.abspath(os.path.join(os.path.dirname(__file__)))
libPath = os.path.join(rootPath, "test.py")
#add libPath to SystemPath
sys.path.insert(0, libPath)

print(sys.path)
```
