licenses(["notice"])  # Apache 2

load(
    "//bazel:envoy_build_system.bzl",
    "envoy_cc_mock",
    "envoy_package",
)

envoy_package()

envoy_cc_mock(
    name = "stats_mocks",
    srcs = ["mocks.cc"],
    hdrs = ["mocks.h"],
    deps = [
        "//include/envoy/stats:stats_interface",
        "//include/envoy/stats:timespan",
        "//include/envoy/thread_local:thread_local_interface",
        "//include/envoy/upstream:cluster_manager_interface",
        "//source/common/stats:fake_symbol_table_lib",
        "//source/common/stats:histogram_lib",
        "//source/common/stats:isolated_store_lib",
        "//source/common/stats:stats_lib",
        "//source/common/stats:store_impl_lib",
        "//test/mocks:common_lib",
        "//test/test_common:global_lib",
    ],
)
