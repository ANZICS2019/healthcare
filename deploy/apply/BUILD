package(default_visibility = ["//visibility:public"])

licenses(["notice"])  # Apache 2.0

go_library(
    name = "apply",
    srcs = [
        "apply.go",
        "gke.go",
    ],
    deps = [
        "//deploy/cft",
        "//deploy/deploymentmanager",
    ],
)

go_test(
    name = "apply_test",
    size = "small",
    srcs = [
        "apply_test.go",
        "gke_test.go",
    ],
    library = ":apply",
    deps = [
        "//deploy/cft",
        "//deploy/deploymentmanager",
        "//third_party/golang/cmp",
        "//third_party/golang/cmp/cmpopts",
        "//third_party/golang/ghodssyaml:yaml",
    ],
)
