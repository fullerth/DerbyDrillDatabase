# GmockSetup
Starting point for a C++ Project with Gmock/Gtest for unit tests and Cmake for configuration.

# Quickstart
```
git clone https://github.com/fullerth/GmockSetup.git
cd GmockSetup
mkdir build && cd build
cmake ..
make
ctest
```

# Cross Compiling
Build this project with a cross compiler by [passing the `-DCMAKE_TOOLCHAIN_FILE` option to Cmake](http://www.vtk.org/Wiki/CMake_Cross_Compiling). The [example toolchain file](CMakeToolChain/Toolchain-RaspberryPi.cmake) shows my setup for a Raspberry Pi target.
