cmake_minimum_required(VERSION 3.12)
project(VideoInputLibrary VERSION 1.0)


set(SOURCES
    videoInput.cpp
)

set(HEADERS
   videoInput.h
)

# Define the target for the videoInput library
add_library(videoInput STATIC ${SOURCES} ${HEADERS})

# Set compiler options
target_compile_options(videoInput PRIVATE -O3)

# Set include directories for the library
target_include_directories(videoInput PUBLIC ./)
