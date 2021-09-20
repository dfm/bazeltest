# bazeltest
Trying to figure out a bazel / LLVM bug

```bash
bazel build --cpu=darwin_arm64 -s @llvm-project//llvm:tblgen
```
