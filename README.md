# Yape 2D - Playground

This repo contains a test app to try the capabilities of [Yape2D](https://github.com/Hegodi/Yape2D) (Yet Another Game Engine).
This Playground includes a graphics user interface which allows you to play and test
different features of the engine. Currently it supports windows and web via emscripten. 

This can give you also an idea of how to integrate
Yape2D in your game.

This app has been made using the [Pixel Game Engine](https://github.com/OneLoneCoder/olcPixelGameEngine).

## Compilation
To compile it you will need:
* C++ compiler

If you want to compile it for emscripten, you will also need:
* emscripten toolchain [emscripten.org](https://emscripten.org/)<br>
    * When you run ```./emsdk activate latest``` you might want to make the change permanent.
* [ninja](https://github.com/ninja-build/ninja/releases) generator

In both cases you can use the makefile included in the project. As you can see, there
is nothing special about it. 

In case you want to to compile using emscripten, from the build folder, run: <br>
* ```emcmake cmake -G Ninja ..```
* ```emmake ninja```

## Running emscripten version
Launch a web server from the folder where you have the html file that emscripten has generated:<br>
*  ```python -m http.server 8000```
Then open a web browser and go to  ```http://localhost:8000/[YOUR_HTML_FILE].html```

You can also find a web version ready to play with in my page [Hegodi](https://hegodi.com)
