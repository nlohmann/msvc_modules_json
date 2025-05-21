This repository contains a small self-contained example of how to use [nlohmann/json](https://github.com/nlohmann/json)
with C++20 modules. The repository contains the `include` folder from
[commit 2d9a251](https://github.com/nlohmann/json/commit/2d9a251266f58b0b08f880c8ad4cc7a9a20014fe). The remaining code
is from [this test case](https://github.com/nlohmann/json/tree/develop/tests/module_cpp20).

It is known to run with GCC 15.1.0 and Clang 20.1.4 with

```shell
cmake -S . -B build -G Ninja
cmake --build build
```

It currently fails to compile with MSVC. An example call is in `.github/workflow.yml`.

See https://github.com/nlohmann/json/issues/3970 for more context.
