load("@rules_cc//cc:defs.bzl", "cc_toolchain", "cc_toolchain_suite")
load(":avr.bzl", "cc_toolchain_config")

cc_toolchain_config(name = "avr_toolchain_config")

cc_toolchain_suite(
    name = "avr_suite",
    toolchains = {
        "avr": ":avr_toolchain",
    },
)

filegroup(name = "empty")

cc_toolchain(
    name = "avr_toolchain",
    all_files = ":empty",
    compiler_files = ":empty",
    dwp_files = ":empty",
    linker_files = ":empty",
    objcopy_files = ":empty",
    strip_files = ":empty",
    supports_param_files = 0,
    toolchain_config = ":avr_toolchain_config",
    toolchain_identifier = "avr-toolchain",
)