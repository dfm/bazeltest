genrule(
    name = "get_cpu_info",
    outs = ["cpu_info.txt"],
    cmd = select({
        "@bazel_tools//src/conditions:darwin_arm64": 'echo "darwin_arm64" > $@',
        "@bazel_tools//src/conditions:darwin_x86_64": 'echo "darwin_x86_64" > $@',
        "//conditions:default": 'echo "unknown" > $@'
    })
)