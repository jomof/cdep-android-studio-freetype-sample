# android-sdl2-gradle-template

## Synopsis

This is an example project for using libSDL2 (https://www.libsdl.org/) in an Android Gradle project using the [CDep](github.com/jomof/cdep)  dependency management tool to download the SDL2 package rather than building it.


## Instructions

All you need to do is clone this project, run CDep, and build.

```
git clone https://github.com/jomof/android-sdl2-gradle-template
cd android-sdl2-gradle-template
./cdep
./gradlew assemble
```
You can also open the project in Android Studio and run it.

## Thanks

This project is forked from https://github.com/stephen47/android-sdl2-gradle-template which was very helpful. 

The example libSDL2 program which draws the square on screen was found at https://stackoverflow.com/questions/21890627/drawing-a-rectangle-with-sdl2/21903973#21903973.

This guide was incredibly useful while I tried to figure out how to get this working: http://lazyfoo.net/tutorials/SDL/52_hello_mobile/android_linux/index.php

The Google NDK example projects were very helpful: https://github.com/googlesamples/android-ndk
