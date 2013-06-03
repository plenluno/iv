# Copyright (c) 2013 Plenluno All rights reserved.

cmake_minimum_required(VERSION 2.8)

project(v8dtoa)

add_library(v8dtoa STATIC
    checks.cc
    conversions.cc
    diy-fp.cc
    fast-dtoa.cc
    platform.cc
    utils.cc
    v8-dtoa.cc
)

target_link_libraries(v8dtoa
    nldtoa
)

set_target_properties(v8dtoa PROPERTIES
    COMPILE_FLAGS ${libj-deps-cflags}
)
