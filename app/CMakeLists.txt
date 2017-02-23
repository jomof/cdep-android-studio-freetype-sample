cmake_minimum_required(VERSION 3.4.1)
list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_LIST_DIR}/../.cdep/modules")

add_library( # Sets the name of the library.
             main

             # Sets the library as a shared library.
             SHARED

             # Provides a relative path to your source file(s).
             # Associated headers in the same location as their source
             # file are automatically included.
             src/main/cpp/main.cpp
             src/main/cpp/SDL_android_main.c)

find_package(cdep-dependencies REQUIRED)
add_all_cdep_dependencies(main)

find_library( # Sets the name of the path variable.
              log-lib

              # Specifies the name of the NDK library that
              # you want CMake to locate.
              log )

target_link_libraries( # Specifies the target library.
                       main

                       # Links the target library to the log library
                       # included in the NDK.
                       ${log-lib})
