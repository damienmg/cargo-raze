"""
cargo-raze crate build file.

DO NOT EDIT! Replaced on runs of cargo-raze
"""
package(default_visibility = ["//vendored/non_cratesio_library/cargo:__subpackages__"])

licenses([
  "notice", # "MIT,Apache-2.0"
])

load(
    "@io_bazel_rules_rust//rust:rust.bzl",
    "rust_library",
    "rust_binary",
    "rust_test",
    "rust_bench_test",
)



rust_library(
    name = "futures",
    crate_root = "src/lib.rs",
    crate_type = "lib",
    srcs = glob(["**/*.rs"]),
    deps = [
        "//vendored/non_cratesio_library/cargo/vendor/futures-channel-0.2.0-alpha:futures_channel",
        "//vendored/non_cratesio_library/cargo/vendor/futures-core-0.2.0-alpha:futures_core",
        "//vendored/non_cratesio_library/cargo/vendor/futures-executor-0.2.0-alpha:futures_executor",
        "//vendored/non_cratesio_library/cargo/vendor/futures-io-0.2.0-alpha:futures_io",
        "//vendored/non_cratesio_library/cargo/vendor/futures-sink-0.2.0-alpha:futures_sink",
        "//vendored/non_cratesio_library/cargo/vendor/futures-stable-0.2.0-alpha:futures_stable",
        "//vendored/non_cratesio_library/cargo/vendor/futures-util-0.2.0-alpha:futures_util",
    ],
    rustc_flags = [
        "--cap-lints allow",
        "--target=x86_64-unknown-linux-gnu",
    ],
    crate_features = [
        "default",
        "futures-core",
        "futures-executor",
        "futures-io",
        "futures-sink",
        "futures-stable",
        "futures-util",
        "std",
    ],
)

