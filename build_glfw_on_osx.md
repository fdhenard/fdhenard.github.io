# How to build GLFW on Mac OSX 10.13 for use in xcode

I didn't want to install GLFW with brew and reference it in my project there.

- install cmake.  I'm using the gui.  `$ brew cask install cmake`
- download source from [here](http://www.glfw.org/download.html)
- extract zip file and move directory to something like `~/dev/native_dependencies/`.  After doing this, my path is `~/dev/native_dependencies/glfw-3.2.1/...`.
- open cmake
- browse source to `~/dev/native_dependencies/`
- create a directory called `build` in `.../native_dependencies/glfw-3.2.1/` so `.../native_dependencies/glfw-3.2.1/build/`
- configure
    - click "configure"
    - select "Unix makefiles" for generator
    - select "Use default native compilers"
    - click "done"


- compile notes here - http://www.glfw.org/docs/latest/compile.html

![image test](https://static.pexels.com/photos/248797/pexels-photo-248797.jpeg)
