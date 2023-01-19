# cmake-intro

This repo is source code for an article titled "Introduction to CMake"
on polishedprogrammer.com and follow-ups.

This project includes a solutions via CMake and standalone GNU
Make. See 'CMakeLists.txt' and 'Makefile'. These are separate ways to
build the C++ code in main.cpp and misc.h.

I included both CMake and GNU Make to contrast two different
approaches. Don't do this normally! I recommend using CMake. Leave
generating makefiles to it! :)

I added a header file called misc.h to show how CMake and GNU Make
handle dependencies. This example is a bit contrived. I would normally
do things differently withe misc.h in both solutions.

## Building with CMake

Execute the following commands from within the root directory of this
repo. You will need CMake version 14 or newer. There are a few ways to
do it. First, let's do things a more modern way.

    cmake -B build
    cmake --build build
 
Another, arguably older, way. Note that I'm assuming CMake will
generate Makefiles in the build directory. This is likely, but not for
sure depending on your platform.

    mkdir build
    cd build
    cmake ..
    cmake --build .

## Building with GNU Make

Execute the following command from within the root directory of this
repo. You will need a current version of Make installed on your
system.

    make

## Summary

There are a number of teachable concepts from this set of files. Parts
of it may not even work for you depending on your OS and
platform. You'll have best luck on a Linux distro that includes
development tools, but I challenge you to try it on Windows or Mac in
different configurations there.

Please see the articles related to this repo on
polishedprogrammer.com. You can search through the list of posts or
use the 'cmake' tag to find it more quickly.

Definitely give CMake a try! I tend to use it in all my projects and
it is really nice most of the time; though I do curse it
occassionally.
