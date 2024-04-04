# RPP-LLVM
C++ coding lab for compiler design

# Build & Run & Pack
Generate the build files using CMake for Release configuration:
```bash
# Windows
cmake -G "MinGW Makefiles" -DCMAKE_INSTALL_PREFIX=out/app -S . -B out/build

# Unix/Linux
cmake -DCMAKE_INSTALL_PREFIX=out/app -S . -B out/build

```

Build the project (Release configuration will be used by default)
```bash
cmake  --build .//out//build -j 12 -v
```

Install the project (Release configuration will be used by default)
```bash
cmake --install .//out//build  --verbose
```

Package the project
```bash
cpack .\out\build  -c Debug --verbose
```