# Directory Tree Printer

Author: Lei Mao (Original Repo) & Aditya Gupta (This Repo)

## Introduction

Printing directory tree is useful to present the direcotry architectures. Such directory trees could often be used in GitHub projects.

Apart from the original one, it now supports .gitignore files too, ie. it will skip the .git directory and other entries in your .gitignore 🎉🎉, also it doesn't have a dependency on boost library now.

## Demo

This is the directory tree of the "Directory Tree Printer" folder.

```
.
├── tree.txt
├── tree_print
├── test_folder
│   ├── file1.txt
│   ├── file2.txt
│   └── folder_1
│       ├── file_3.txt
│       ├── file1.txt
│       ├── file2.txt
│       └── folder_2
│           ├── file1.txt
│           ├── file2.txt
│           └── folder_2
│               ├── file1.txt
│               ├── file2.txt
│               └── folder_2
├── tree_print.cpp
├── CMakeLists.txt
├── demo.txt
├── README.md
├── tree.h
└── tree.cpp
```

## Usage

```shell
./dtree .
./dtree DIRECTORY_NAME_OR_PATH
```

## Building
----
To compile the from the source code, simply run:
```shell
mkdir build && cd build
cmake ..
cmake --build .
```

You will get a `dtree` executable then.

## Notes
* You need a compiler supporting C++17
* Linux has similar packages to present directory tree,

    On Ubuntu:
    ```shell
    sudo apt install tree
    ```
