# C++ Binary Fixed-Point Arithmetic

[![Build Status](https://travis-ci.org/johnmcfarlane/fixed_point.svg)](https://travis-ci.org/johnmcfarlane/fixed_point)
[![Build status](https://ci.appveyor.com/api/projects/status/u8gvlnbi8puo2eee?svg=true)](https://ci.appveyor.com/project/johnmcfarlane/fixed-point)

## Introduction

The [fixed_point](https://github.com/johnmcfarlane/fixed_point)
library is designed to represent binary fixed-point real numbers using
built-in integer types. It is developed as part of
[SG14](https://groups.google.com/a/isocpp.org/forum/#!forum/sg14) and
SG6.
For an overview of the API, see draft proposal,
[LEWG, EWG, SG14, SG6: P0037](http://johnmcfarlane.github.io/fixed_point/docs/papers/p0037.html).

## Instructions

### Download

The library is hosted on [GitHub](https://github.com/):

    git clone https://github.com/johnmcfarlane/fixed_point.git --recursive
    cd fixed_point

### Linux

Tested on Debian GNU/Linux 8.2 using GCC 4.9 and Clang 3.5

To build:

    cmake -DCMAKE_BUILD_TYPE=Release
    make

To disable exception handling, add `-DEXCEPTIONS=OFF` to the `cmake` command:

    cmake -DCMAKE_BUILD_TYPE=Release -DEXCEPTIONS=OFF
    make

To run tests:

    ./run_tests

To run benchmarks:

    ./run_benchmarks

### Windows

Tested on Windows 7 Professional. Requires version 14.0 of MSBuild. (You can probably find it in `c:\Program Files (x86)\MSBuild\14.0\Bin`.)

    msbuild vs\fixed_point_test.sln
