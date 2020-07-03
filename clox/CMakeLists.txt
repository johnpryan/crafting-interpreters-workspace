cmake_minimum_required(VERSION 3.16)
project(clox C)

set(CMAKE_C_STANDARD 99)

add_executable(
        clox
        chunk.c
        chunk.h
        common.h
        compiler.c
        compiler.h
        debug.c
        debug.h
        main.c
        memory.c
        memory.h
        scanner.c
        scanner.h
        value.c
        value.h
        vm.c
        vm.h
        object.h object.c)
