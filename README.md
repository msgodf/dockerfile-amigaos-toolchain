# Dockerfile for building the AmigaOS toolchain

This is a convenient way to build the AmigaOS cross compiler toolchain written by Krystian Bacławski (https://github.com/cahirwpz/amigaos-cross-toolchain/).

It can run in a Docker container on x86 and the Raspberry Pi.

## Building for x86

`docker build .`

## Building for the Raspberry Pi

`docker build -f Dockerfile-rpi .`
