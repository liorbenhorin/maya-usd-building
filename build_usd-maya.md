The build.py must be called via the 
"x64 Native Tools Command Prompt"

looks like when passing the 'workspace' argument as the last positional argument, the code is failing..., so, I'm just running without it, and files are landing to maya-usd/Files



```
set PATH=%PATH%;C:\Python27;C:\Python27\Scripts
d:
cd D:\development\USD_DEV\maya-usd
python build.py --generator Ninja --maya-location C:/Program Files/Autodesk/Maya2019 --pxrusd-location D:/development/USD_DEV/build/USD --devkit-location D:/development/USD_DEV/maya-devkit-update2 --build-args="-DCMAKE_MAKE_PROGRAM=D:/development/USD_DEV/ninja/ninja.exe"
```
_Note the forward slashes in the build.py arguments_

To allow maya to load the plug-ins, we have to add this into maya.env
```MAYA_MODULE_PATH=D:\development\USD_DEV\build\maya-usd\RelWithDebInfo```