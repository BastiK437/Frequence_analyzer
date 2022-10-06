cmake_minimum_required(VERSION 3.13)  # CMake version check
project(Frequence_analyzer)

# Add executable target with source files listed in SOURCE_FILES variable
add_executable(Frequence_analyzer src/main.c)

find_library(SOUNDIO_LIB soundio)
target_link_libraries(Frequence_analyzer PRIVATE "${SOUNDIO_LIB}")