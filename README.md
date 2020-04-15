# maya-usd-building
Collection of instructions for building maya-usd

# Pixar USD

This is the USD core repository, which is the basic building block for all USD driven plug-ins

[https://graphics.pixar.com/usd/docs/index.html]()

[https://github.com/PixarAnimationStudios/USD]()

[https://www.manicmachinegames.com/blog/2019/1/10/tutorial-setting-up-and-building-pixars-usd-on-windows]()

### Build (Windows 10)

The instructions are all very clear and should be followed to the latter.

- Python version should be 2.7.12
- No other python should be in the PATH
- Pip install the following:

``$ pip install pyd PySide PyOpenGL PyOpenGL_accelerate``

- when calling buil-usd.py, we will need to pass the following arguments for it to be able to build "boost" successfully: [https://github.com/Autodesk/maya-usd/blob/dev/doc/build.md#additional-build-instruction]()

- At the time of writing this, I have been using [v20.02](https://github.com/PixarAnimationStudios/USD/releases/tag/v20.02) of USD. Looks like the release has a bug on Windows 10:
[https://github.com/PixarAnimationStudios/USD/issues/1133](https://github.com/PixarAnimationStudios/USD/issues/1133) 



## maya-usd

This is the Autodesk maintained repository that is now the home of both Pixar's usd-maya plug-in, and Animal logic's usd-maya plug-in
The repo also containes the Autodesk usd-maya plug-in.

https://github.com/Autodesk/maya-usd
https://github.com/Autodesk/maya-usd/blob/dev/doc/build.md
