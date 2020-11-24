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

# Configuring this module
Once the module is registered, navigate to `Inkycal/server` and run the flask-server with:
`flask run --host=0.0.0.0`

The web-UI should now be available at `http://raspberrypi.local:5000/`. If this does not work, you can manually use the IP address instead: `http://192.168.1.142:5000/`

Copy the generated settings.json file to your raspberry Pi (VNC/ WinSCP). 
If you don't have access to the Raspberry Pi via VNC/ WinSCP, you can copy the settings.json file to the microSD card instead. After inkycal starts, it will use the new settings.json file.

# How to remove this module
```python3
# In python, run the following commands:
from inkycal import Inkycal
Inkycal.remove_module('filename.py') # where filename.py is the name of your third-party module in Inkycal/inkycal/modules
# If everything went well, you'll see a printed message without red lines.
```
