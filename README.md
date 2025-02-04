# Yape 2D - Playground

This repo contains a test app to try the capabilities of Yape2D (Yet Another Game Engine).
The Playground includes a graphics user interface which allows you to play and test
different features of the engine. Currently it supports windwos and web via emscripten. 

To compile it you will need:
* C++ compiler

If you want to compile it for emscripten, you will also need:
* emscripten toolchain [emscripten.org](https://emscripten.org/)<br>
    * When you run ```./emsdk activate latest``` you might want to make the change permanent.
* [ninja](https://github.com/ninja-build/ninja/releases) generator

## Compilation
In both cases you can use the makefile included in the project. As you can see, there
is nothing special about it. 

In case you want to to compile using emscripten, from the build folder, run: <br>
* ```emcmake cmake -G Ninja ..```
* ```emmake ninja```

## Running emscripten version
Launch a web server from the folder where you have the html file that emscripten has generated:<br>
*  ```python -m http.server 8000```
Then open a web browser and go to  ```http://localhost:8000/[YOUR_HTML_FILE].html```

