Run 

```bash
bazel build //... --cpu=arm64-v8a --host_crosstool_top=@bazel_tools//tools/cpp:toolchain --crosstool_top=@androidndk//:toolchain-libcpp --cxxopt=-std=c++14
```

Expected result: build success.
Result: error: invalid argument '-std=c++14' not allowed with 'C'
