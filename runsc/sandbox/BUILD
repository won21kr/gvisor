package(licenses = ["notice"])  # Apache 2.0

load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "sandbox",
    srcs = [
        "chroot.go",
        "network.go",
        "sandbox.go",
    ],
    importpath = "gvisor.googlesource.com/gvisor/runsc/sandbox",
    visibility = [
        "//runsc:__subpackages__",
    ],
    deps = [
        "//pkg/control/client",
        "//pkg/control/server",
        "//pkg/log",
        "//pkg/sentry/control",
        "//pkg/sentry/platform/kvm",
        "//pkg/urpc",
        "//runsc/boot",
        "//runsc/console",
        "//runsc/specutils",
        "@com_github_cenkalti_backoff//:go_default_library",
        "@com_github_opencontainers_runtime-spec//specs-go:go_default_library",
        "@com_github_syndtr_gocapability//capability:go_default_library",
        "@com_github_vishvananda_netlink//:go_default_library",
    ],
)
