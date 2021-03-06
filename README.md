# Freetype and SDL2 on Android
This is a sample project that combines Freetype (http://www.freetype.org) and SDL2 (https://www.libsdl.org) together in an Android Gradle project using the [CDep](https://github.com/jomof/cdep) dependency management tool to download the Freetype and SDL2 packages rather than building them. 

[![Build Status](https://travis-ci.org/jomof/cdep-android-studio-freetype-sample.svg?branch=master)](https://travis-ci.org/jomof/cdep-android-studio-freetype-sample) [![Freetype Status](https://cdep-io.github.io/com.github.jomof/freetype/latest/latest.svg)](https://github.com/jomof/freetype/releases/latest) [![CDep Status](https://cdep-io.github.io/com.github.jomof/sdl2/latest/latest.svg)](https://github.com/jomof/sdl2/releases/latest)

![Screen Shot](screenshot.jpg)

## Instructions

All you need to do is clone this project, run CDep, and build.

```
git clone https://github.com/jomof/cdep-android-studio-freetype-sample.git
cd cdep-android-studio-freetype-sample
./cdep  # Downloads dependencies referenced in cdep.yml
./gradlew assemble
```
You can also open the project in Android Studio and run it.

## Thanks
The main loop that demonstrates Freetype with SDL2 is adapted from https://github.com/wutipong/drawtext-sdl2-freetype2-harfbuzz/blob/master/sdl-ft-1/main.cpp.

This project itself is orginally forked from https://github.com/stephen47/android-sdl2-gradle-template which was very helpful. 

### The author of that project also had these thanks.

The example libSDL2 program which draws the square on screen was found at https://stackoverflow.com/questions/21890627/drawing-a-rectangle-with-sdl2/21903973#21903973.

This guide was incredibly useful while I tried to figure out how to get this working: http://lazyfoo.net/tutorials/SDL/52_hello_mobile/android_linux/index.php

The Google NDK example projects were very helpful: https://github.com/googlesamples/android-ndk
