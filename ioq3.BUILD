load("@rules_foreign_cc//foreign_cc:defs.bzl", "cmake")

filegroup(
    name = "srcs",
    srcs = glob(["**"]),
    visibility = ["//visibility:public"],
)

cmake(
    name = "server",
    cache_entries = {
        "CMAKE_BUILD_TYPE": "Release",
        "BUILD_CLIENT": "false",
    },
    lib_source = ":srcs",
    out_bin_dir = "",
    out_binaries = ["ioq3ded"],
    visibility = ["//visibility:public"],
)
