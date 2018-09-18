package(default_visibility = ["//tools/compiler_e6500:__pkg__"])

filegroup(
    name = "gcc",
    srcs = [
        "powerpc64-fsl-linux-gcc",
        "@toolchain_e6500//:gcc",
    ],
)

filegroup(
    name = "ar",
    srcs = [
        "powerpc64-fsl-linux-ar",
        "@toolchain_e6500//:ar",
    ],
)

filegroup(
    name = "ld",
    srcs = [
        "powerpc64-fsl-linux-ld",
        "@toolchain_e6500//:ld",
    ],
)

filegroup(
    name = "nm",
    srcs = [
        "powerpc64-fsl-linux-nm",
        "@toolchain_e6500//:nm",
    ],
)

filegroup(
    name = "objcopy",
    srcs = [
        "powerpc64-fsl-linux-objcopy",
        "@toolchain_e6500//:objcopy",
    ],
)

filegroup(
    name = "objdump",
    srcs = [
        "powerpc64-fsl-linux-objdump",
        "@toolchain_e6500//:objdump",
    ],
)

filegroup(
    name = "strip",
    srcs = [
        "powerpc64-fsl-linux-strip",
        "@toolchain_e6500//:strip",
    ],
)

filegroup(
    name = "as",
    srcs = [
        "powerpc64-fsl-linux-as",
        "@toolchain_e6500//:as",
    ],
)

filegroup(
    name = "tool-wrappers",
    srcs = [
        ":ar",
        ":as",
        ":gcc",
        ":ld",
        ":nm",
        ":objcopy",
        ":objdump",
        ":strip",
    ],
)
