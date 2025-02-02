# TDLib C++ basic usage examples

TDLib should be prebuilt and installed to local subdirectory `td/`:
```
cd <path to TDLib sources>
mkdir build
cd build
cmake -DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFIX:PATH=../example/cpp/td ..
cmake --build . --target install
```
Also see [building](https://github.com/tdlib/td#building) for additional details on TDLib building.

Then you can build the examples:
```
cd <path to TDLib sources>/example/cpp
mkdir build
cd build
cmake -DCMAKE_BUILD_TYPE=Release -DTonlib_DIR=<full path to TDLib sources>/example/cpp/tonlib/lib/cmake/Tonlib ..
cmake --build .
```

Documentation for all available classes and methods can be found at https://core.telegram.org/tdlib/docs.

To run `tdjson_example` you may need to manually copy a `tdjson` shared library from `td/bin` to a directory containing built binaries.
