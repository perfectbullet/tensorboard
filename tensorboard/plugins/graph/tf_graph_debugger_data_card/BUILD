package(default_visibility = ["//tensorboard:internal"])

load("//tensorboard/defs:defs.bzl", "tensorboard_webcomponent_library")
load("//tensorboard/defs:web.bzl", "tf_web_library")

licenses(["notice"])  # Apache 2.0

tf_web_library(
    name = "tf_graph_debugger_data_card",
    srcs = [
        "tf-graph-debugger-data-card.html",
    ],
    path = "/tf-graph-debugger-data-card",
    deps = [
        "//tensorboard/components/tf_dashboard_common",
        "//tensorboard/components/tf_imports:polymer",
        "//tensorboard/plugins/graph/tf_graph_common",
        "@org_polymer_paper_material",
        "@org_polymer_paper_slider",
        "@org_polymer_paper_spinner",
        "@org_polymer_paper_toggle_button",
    ],
)

tensorboard_webcomponent_library(
    name = "legacy",
    srcs = [":tf_graph_debugger_data_card"],
    destdir = "tf-graph-debugger-data-card",
    deps = [
        "//tensorboard/components/tf_dashboard_common:legacy",
        "//tensorboard/components/tf_imports:polymer_lib",
        "//tensorboard/plugins/graph/tf_graph_common:legacy",
        "//third_party/javascript/polymer/v2/paper-material:lib",
        "//third_party/javascript/polymer/v2/paper-slider:lib",
        "//third_party/javascript/polymer/v2/paper-spinner:lib",
        "//third_party/javascript/polymer/v2/paper-toggle-button:lib",
    ],
)
