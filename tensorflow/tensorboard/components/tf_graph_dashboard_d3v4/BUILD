package(default_visibility = ["//tensorflow:internal"])

load("@io_bazel_rules_closure//closure:defs.bzl", "web_library")
load("//tensorflow/tensorboard:defs.bzl", "tensorboard_ts_library")
load("//tensorflow/tensorboard:defs.bzl", "tensorboard_webcomponent_library")

licenses(["notice"])  # Apache 2.0

web_library(
    name = "tf_graph_dashboard_d3v4",
    srcs = [
        "tf-graph-dashboard.html",
    ],
    path = "/tf-graph-dashboard",
    deps = [
        "//tensorflow/tensorboard/components/tf_backend_d3v4",
        "//tensorflow/tensorboard/components/tf_dashboard_common_d3v4",
        "//tensorflow/tensorboard/components/tf_graph_board_d3v4",
        "//tensorflow/tensorboard/components/tf_graph_controls_d3v4",
        "//tensorflow/tensorboard/components/tf_graph_d3v4",
        "//tensorflow/tensorboard/components/tf_graph_loader_d3v4",
        "@org_polymer",
    ],
)

filegroup(
    name = "all_files",
    srcs = glob(["**"]),
    tags = ["notsan"],
)
