# This is the entry point for --crosstool_top.  Toolchains are found
# by lopping off the name of --crosstool_top and searching for
# 'cc-compiler-${CPU}' in this BUILD file, where CPU is the target CPU
# specified in --cpu.
#
# This file group should include
#   * all cc_toolchain targets supported
#   * all file groups that said cc_toolchain might refer to,
# including the default_grte_top setting in the CROSSTOOL
# protobuf.
filegroup(
    name = "toolchain_fg",
    srcs = [
        ":cc-compiler-e6500",
        ":cc-compiler-k8",
        ":e6500_all_files",
        "@toolchain_e6500//:compiler_components",
    ],
)

cc_toolchain_suite(
    name = "toolchain",
    # target_cpu | compiler
    toolchains = {
        "e6500|gcc": "cc-compiler-e6500",
        "k8|compiler": "cc-compiler-k8",
    },
)

filegroup(
    name = "e6500_all_files",
    srcs = [
        "//tools/compiler_e6500/e6500_gcc:tool-wrappers",
        "@toolchain_e6500//:compiler_pieces",
    ],
)

filegroup(
    name = "e6500_linker_files",
    srcs = [
        "//tools/compiler_e6500/e6500_gcc:ar",
        "//tools/compiler_e6500/e6500_gcc:gcc",
        "//tools/compiler_e6500/e6500_gcc:ld",
        "@toolchain_e6500//:compiler_pieces",
    ],
)

filegroup(
    name = "e6500_compiler_files",
    srcs = [
        "//tools/compiler_e6500/e6500_gcc:as",
        "//tools/compiler_e6500/e6500_gcc:gcc",
        "//tools/compiler_e6500/e6500_gcc:ld",
    ],
)

filegroup(
    name = "empty",
    srcs = [],
)

cc_toolchain(
    name = "cc-compiler-e6500",
    all_files = ":e6500_all_files",
    ar_files = "//tools/compiler_e6500/e6500_gcc:ar",
    as_files = "//tools/compiler_e6500/e6500_gcc:as",
    compiler_files = ":e6500_compiler_files",
    cpu = "e6500",
    dwp_files = ":empty",
    dynamic_runtime_libs = [":empty"],
    linker_files = ":e6500_linker_files",
    objcopy_files = "//tools/compiler_e6500/e6500_gcc:objcopy",
    static_runtime_libs = [":empty"],
    strip_files = "//tools/compiler_e6500/e6500_gcc:strip",
    supports_param_files = 1,
    visibility = ["//visibility:public"],
)

cc_toolchain(
    name = "cc-compiler-k8",
    all_files = ":empty",
    ar_files = ":empty",
    as_files = ":empty",
    compiler_files = ":empty",
    cpu = "local",
    dwp_files = ":empty",
    dynamic_runtime_libs = [":empty"],
    linker_files = ":empty",
    objcopy_files = ":empty",
    static_runtime_libs = [":empty"],
    strip_files = ":empty",
    supports_param_files = 1,
)
