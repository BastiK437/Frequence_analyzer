# Frequence_analyzer

## CMake

- mkdir build && cd build
- cmake ..
- cmake --build .

## soundlibio

Soundlibio must have been installed on the system. Check soundlib.io for more information. 

### Dependencie for CMake

Add the following in the CMakeLists.txt:

````
find_library(SOUNDIO_LIB soundio)
target_link_libraries(Frequence_analyzer PRIVATE "${SOUNDIO_LIB}")
````