## ```install_gis_packages.py```
Install script for installing the python GIS tool chain in an Anaconda environment.  

### to run
```
>python install_gis_packages.py
```
in the screen output, you should see the message
```The following NEW packages will be INSTALLED:```, followed by a list of packages, and then messages about fetching, extracting and linking the packages.

### to test
##### activate the gis environment  

on Windows:  

```
>activate gis
```

on OSX  

```
>source activate gis
```
(gis) will be added before the command prompt.  
then  

```
>python run_tests.py
```
**Note: ```run_tests.py``` must be run from the "scripts" folder** (and the "tests" folder, which contains the tests, must be present at the same level as scripts; i.e. so that
```cd ../tests``` would change the directory from scripts to tests.)
The test script should report "OK" after it has ran.

### to uninstall
switch back to the default environment with  

```  
>deactivate
```
on windows, or

```  
>source deactivate  
```
on OSX. Then  

```
>conda env remove -n gis  
```

