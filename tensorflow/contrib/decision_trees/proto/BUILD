package(default_visibility = ["//visibility:public"])

licenses(["notice"])  # Apache 2.0

exports_files([
    "LICENSE",
    "generic_tree_model_proto.swig",
])

load("//tensorflow/core:platform/default/build_config.bzl", "tf_proto_library")

tf_proto_library(
    name = "generic_tree_model",
    srcs = ["generic_tree_model.proto"],
    cc_api_version = 2,
    go_api_version = 2,
    java_api_version = 2,
)

tf_proto_library(
    name = "generic_tree_model_extensions",
    srcs = ["generic_tree_model_extensions.proto"],
    cc_api_version = 2,
    go_api_version = 2,
    protodeps = [":generic_tree_model"],
)
