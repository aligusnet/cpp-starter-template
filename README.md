# C++ Starter Template Project

This is a C++ starter project template for getting up and running with C++ quickly.

## Using conan for dependencies.

### Install conan

```sh
> python -m pip install conan
```

### Configure project

```sh
> conan profile detect  # in case if no conan profiles created
> conan install . --output-folder=build --build=missing
> cd build
> cmake .. -DCMAKE_TOOLCHAIN_FILE=conan_toolchain.cmake -DCMAKE_BUILD_TYPE=Release
> cmake --build .
> cd ..
> code .
```

Use Conan's CMake presets in VS Code.