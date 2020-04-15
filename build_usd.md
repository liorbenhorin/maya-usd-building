

The build_usd.py must be called via the 
"x64 Native Tools Command Prompt"

Add python to the PATH

``set PATH=%PATH%;C:\Python27;C:\Python27\Scripts``

navigate to the USD repo

``python build_scripts\build_usd.py "D:\development\USD_DEV\build\USD" --build-args boost,"--with-date_time --with-thread --with-system --with-filesystem"``


After a successful build, run (From a standard bash):

```
d:
cd development\USD_DEV\USD-20.02\USD
set PYTHONPATH=D:\development\USD_DEV\build\USD\lib\python
set PATH=%PATH%;D:\development\USD_DEV\build\USD\lib;D:\development\USD_DEV\build\USD\bin
set PATH=%PATH%;C:\Python27;C:\Python27\Scripts
usdview extras/usd/tutorials/convertingLayerFormats/Sphere.usda
```
