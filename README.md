# Name of your module
This is third-party module for the inkycal project for release 2.0.0

First, add a **SCREENSHOT** (This is very important!)

Explain these things in a few sentences:
* what this module does (why did you put effor into making this?)
* what it requires (dependencies, account at some website etc.)
* how to set it up (with a sample config)
* development status (are you maintaining it?)

# Installation instructions
How to install the module.

1) Navigate to the modules directory
`cd Inkycal/inkycal/modules`

2) Download the third-party module:
```bash
# The URL is the rawfile url. e.g. open mymodule.py, then click on [raw] to see the rawfile-url
wget https://raw.githubusercontent.com/aceisace/inkycal_template/master/mymodule.py
```

3) Register this module in Inkycal
```python3
# In python, type the following commands:
from inkycal import Inkycal
inkycal.add_module('/full/path/to/your/module.py')
# If everything went well, you should see a printed message without red lines.
```


# How to remove this module
```python3
# In python, run the following commands:
from inkycal import Inkycal
Inkycal.remove_module('filename.py') # where filename.py is the name of your third-party module in Inkycal/inkycal/modules
# If everything went well, you'll see a printed message without red lines.
```
