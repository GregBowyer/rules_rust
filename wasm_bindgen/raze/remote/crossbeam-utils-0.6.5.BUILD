"""
cargo-raze crate build file.

DO NOT EDIT! Replaced on runs of cargo-raze
"""

package(default_visibility = [
    # Public for visibility by "@raze__crate__version//" targets.
    #
    # Prefer access through "//wasm_bindgen/raze", which limits external
    # visibility to explicit Cargo.toml dependencies.
    "//visibility:public",
])

licenses([
    "notice",  # "MIT,Apache-2.0"
])

load(
    "@io_bazel_rules_rust//rust:rust.bzl",
    "rust_binary",
    "rust_library",
    "rust_test",
)

# Unsupported target "atomic_cell" with type "bench" omitted
# Unsupported target "atomic_cell" with type "test" omitted
# Unsupported target "cache_padded" with type "test" omitted

rust_library(
    name = "crossbeam_utils",
    srcs = glob(["**/*.rs"]),
    crate_features = [
        "default",
        "lazy_static",
        "std",
    ],
    crate_root = "src/lib.rs",
    crate_type = "lib",
    edition = "2015",
    rustc_flags = [
        "--cap-lints=allow",
    ],
    version = "0.6.5",
    deps = [
        "@raze__cfg_if__0_1_9//:cfg_if",
        "@raze__lazy_static__1_3_0//:lazy_static",
    ],
)

# Unsupported target "parker" with type "test" omitted
# Unsupported target "sharded_lock" with type "test" omitted
# Unsupported target "thread" with type "test" omitted
# Unsupported target "wait_group" with type "test" omitted
