# Init CMake project

Create cmake file
```
touch CMakeLists.txt #
```

Create output directory
```
mkdir -p out/build
```

Insall cmake: source to project directory
```
cmake -S ../../ -B .
```

Try to build project:
```
cmake -S . -B out/build
```
 
Entry the `out/build` to build programming
```
cd out/build/
make
```

# Library and subdirectory

Build from project directory: `make -C out/build`

Add other file to cmake build
```
add_executable(${PROJECT_NAME} main.cpp <new_file.cpp>)
```

Each subdirectory should have `CMakeLists.txt` file
