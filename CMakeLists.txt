cmake_minimum_required(VERSION 3.12)
project(dtree
        VERSION 2.1
        DESCRIPTION "Alternative to `tree` command that honours .gitignore"
    )

set(CMAKE_CXX_STANDARD 17)
set(SOURCES tree.cpp "main.cpp")
add_executable(dtree ${SOURCES})
