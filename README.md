cpp_rakefile
============

An example c++ project that uses a Rakefile with a few helpful tasks.

Rake Tasks:
```
devops001@ubuntu:~/github/cpp_rakefile> rake -T
rake addclass[name]  # Creates a new c++ class (.h & .cpp files) with the given NAME rake variable.
rake clean           # Remove all src/*.o and bin/*.exe files
rake debug           # Debug bin/main.exe
rake default         # Compile bin/main.exe
rake run             # Compile and run bin/main.exe
rake setup           # Create directories: src, inc, bin, doc, logs
```

Example of adding a class:
```
devops001@ubuntu:~/github/cpp_rakefile> rake addclass["WaterBuffalo"]
class:   WaterBuffalo
header:  /home/devops001/github/cpp_rakefile/inc/WaterBuffalo.h
source:  /home/devops001/github/cpp_rakefile/src/WaterBuffalo.cpp

devops001@ubuntu:~/github/cpp_rakefile> tree
.
├── bin
├── doc
├── inc
│   └── WaterBuffalo.h
├── LICENSE
├── logs
├── Rakefile
└── src
    ├── main.cpp
    └── WaterBuffalo.cpp

5 directories, 5 files
```
