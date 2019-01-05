# Design of the EEGsynth

The design of the EEGsynth is modular, directly inspired by 
[modular synthesizers](https://en.wikipedia.org/wiki/Modular_synthesizer) (see picture below). 
Every module does a specific task. Each module consists of a python script, and is contained in its own directory. 
For instance, in [eegsynth\modules\launchcontrol](https://github.com/eegsynth/eegsynth/modules/launchcontrol) we find:
 * [launchcontrol.py](https://github.com/eegsynth/eegsynth/modules/launchcontrol/launchcontrol.py) 
 is the [Python](https://www.python.org/) script. Read more about the python scripts [here](scripts.md).
 * [launchcontrol.ini](https://github.com/eegsynth/eegsynth/modules/launchcontrol/launchcontrol.ini)
 is the initialization file setting the parameters and the way it's connected. Read more about the ini files [here](inifile.md)
 * [README.MD](https://github.com/eegsynth/eegsynth/modules/launchcontrol/README.MD) is the explanation of the module in [markdown](https://en.wikipedia.org/wiki/Markdown) format 

Similarly as in modular synthesizers, the EEGsynth functions when several modules are interconnected, sending 
and receiving information from each other. Similarly as in modular synthesizers, we call this patching.
Read more about how we implement patching [here](patching.md)

_Continue reading: [Python scripts](scripts.md)_