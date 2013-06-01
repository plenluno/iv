# Copyright (c) 2013 Plenluno All rights reserved.

cmake_minimum_required(VERSION 2.8)

project(nldtoa)

add_library(nldtoa STATIC
    netlib_dtoa.c
)
