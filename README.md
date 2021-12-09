# IMGUI library generator for SDL2 and opengl3

This repo contains the files to create a static imgui library   
The library will work with SDL2 and opengl3

**The library itself is for my own use, so dont expect a great makefile or organization**

## Instalation
Install in your system SDL2 and opengl  

In your proyect, create a `lib` folder and put the folder there  
Then, use `make` to generate the static library  
Ones done that, include the library in your code and in your makefile.  
You will need dependencies, so make sure you link the correct ones

**Linking example**: `-L./lib/imgui -lSDL2 -lSDL2main -lz -lGL -limgui -ldl`

## Implementing in the code
To use the library just include the respective headers

    ...
    #include <imgui/src/imgui.h>
    #include <imgui/src/imgui_impl_sdl.h>
    #include <imgui/src/imgui_impl_opengl3.h>
    ...

**NOTE:** This library does not have apart the headerfiles, they will be mixed with the .cpp and .o files
