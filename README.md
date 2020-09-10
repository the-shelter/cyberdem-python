# Cyber Data Exchange Model (CyberDEM) Python Package

## Overview
CyberDEM Python provides a Python API for the [Cyber Data Exchange Model](https://www.sisostds.org/StandardsActivities/DevelopmentGroups/CyberDEMPDG.aspx) (CyberDEM). CyberDEM Python provides methods to instantiate CyberDEM objects and events, serialize and deserialize objects and events, and manipulate instantiated objects. It also provides basic searching and file management methods. 

## Status

CyberDEM Python is based on the CyberDEM standard that is currently in DRAFT format, and therefore subject to change. 

## Getting Started

These instructions will help you install a copy of the package on your local machine.

### Installing

1. Download CyberDEM Python and unzip the download folder
2. From within the top-level cyberdem folder (where [setup.py](setup.py) is located) run
```
$ pip3 install .
```

3. To test that cyberdem is installed properly run

```
$ python3
>>> from cyberdem import base
>>> print(base.System())
System(
    id: 3bb3512e-dc75-4b86-b234-25040a79b9b9
)
```

You may also try running the example.py file downloaded with the zip file.

```
$ python3 example.py
Creating new FileSystem path ./test-fs.

QUERY 1
--------
['description', 'id', 'name', 'version', '_type']
('Rapid SCADA software', '0f717dfa-...', 'Rapid SCADA', '5', 'Application')
('PfSense Firewall', '2720359e-...', 'PfSense', '2.4.2', 'Application')
(None, '2f6ac399-...', None, None, 'Application')
(None, 'd36e99ce-...', None, None, 'Application')
('Firefox browser', 'df8478d6-...', 'Firefox', '60', 'Application')
(None, '0eaacdbc-...', None, None, 'Application')
(None, '6265eb88-...', None, None, 'Application')

[expected output]
```
You will see a folder called "test-fs" in the directory in which you ran the [example.py](example.py) script. This folder has subfolders containing each type of Cyber DEM object/event.

### Documentation

The code documentation can be found as a pdf [here](assets/cyberdempython.pdf).

## License

Copyright 2020 Carnegie Mellon University. See the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgements

- [SISO Cyber DEM Product Development Group](https://www.sisostds.org/StandardsActivities/DevelopmentGroups/CyberDEMPDG.aspx)