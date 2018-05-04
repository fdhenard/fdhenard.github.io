# Xcode setup for Learn OpenGL Tutorials

The instructions worked on 5/4/18 on this system:

- Mac OSX High Sierra 10.13
- Xcode 9.3

## instructions

- build glfw - instructions are [here](build_glfw_on_osx.md)
- open Xcode
- select menus - File / New / Project
- Command Line Tool
- Next
- Product Name...
- Language: C++
- Next - creates project
- add OpenGL Framework to link phase
    - select the project (root level of project explorer on left)
    - select "Build Phases" in top center
    - in "Link Binary with Libraries"
    - "+" / Add Other
    - type "OpenGL" in search
    - double click OpenGL.framework
- GLFW
    - add to search paths
        - select the project (root level of project explorer on left)
        - select "build settings" in top center
        - in the search box in build settings, type "search"
        - Header Search Paths - add path `/Users/<you>/dev/native_dependencies/glfw-3.2.1/include`
        - Library Search Paths - add path `/Users/<you>/dev/native_dependencies/build/src`
    - add to link phase
        - select the project (root level of project explorer on left)
        - select "Build Phases" in top center
        - in "Link Binary with Libraries"
        - "+" / Add Other
        - select `~/dev/native_dependencies/glfw-3.2.1/build/src/libglfw.3.2.dylib`
- GLAD
    - [the tutorial](https://learnopengl.com/Getting-started/Creating-a-window) is good to follow for instructions on GLAD.  Use the web service, to create the GLAD zip file, and download.
    - extract the zip to `~/dev/native_dependencies/glad`
    - add glad header search path
        - again go to "build settings" / Header Search Paths
        - add path `/Users/<you>/dev/native_dependencies/glad/include`
    - add glad c file
        - go to menu - File / "Add files to <your project>"
        - select `~/dev/native_dependencies/glad/src/glad.c`



