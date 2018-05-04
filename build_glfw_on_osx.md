# How to build GLFW on Mac OSX 10.13 for use in xcode

The Learn OpenGL tutorial said to build it instead of getting a build.  That could be done with brew, but could also be done by building the source with cmake.  Here's how I did it.

Compile notes are [here](http://www.glfw.org/docs/latest/compile.html)

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
- This creates a list of entries
- check the `BUILD_SHARED_LIBS` entry.
- click "generate"
- make
    - go to terminal
    - `$ cd ~/dev/native_dependencies/glfw-3.2.1/build/`
    - `$ make`
- dynamic libraries should be built.  You should be able to see them in `~/dev/native_dependencies/glfw-3.2.1/build/src/`

Log issues or make pull requests to this post [here](https://github.com/fdhenard/fdhenard.github.io)

This is my first attempt with github pages.  I was testing adding an image, and I like it, so I'm just going to leave it here.

![image test](https://static.pexels.com/photos/248797/pexels-photo-248797.jpeg)
