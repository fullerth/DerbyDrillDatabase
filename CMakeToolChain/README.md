

The cmake toolchain file contains local configuration it should not be checked 
into source control. [Toolchain-RaspberryPi.cmake](Toolchain-RaspberryPi.cmake) 
is included in this repo as a starting point for new projects. After cloning, 
it should be removed from the repo with `git rm` and added to 
`.gitignore`.

Open [Toolchain-RaspberryPi.cmake](Toolchain-RaspberryPi.cmake) in your 
favourite editor. Change the `CMAKE_C_COMPILER` and `CMAKE_CXX_COMPILER` 
variables to point to local copies of your C and C++ cross compiler binary. Use 
the following command from the root of the repo to generate the makefile

```bash
mkdir -p build & cd build
cmake .. -DCMAKE_TOOLCHAIN_FILE=../CMakeToolChain/Toolchain-RaspberryPi.cmake
```
