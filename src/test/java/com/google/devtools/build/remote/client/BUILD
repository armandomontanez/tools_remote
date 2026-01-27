load("@rules_java//java:java_test.bzl", "java_test")

java_test(
    name = "GrpcRemoteCacheTest",
    srcs = [
        "FakeImmutableCacheByteStreamImpl.java",
        "GrpcRemoteCacheTest.java",
    ],
    deps = [
        "//src/main/java/com/google/devtools/build/remote/client",
        "//third_party/remote-apis:build_bazel_remote_execution_v2_remote_execution_java_grpc",
        "@bazel_remote_apis//build/bazel/remote/execution/v2:remote_execution_java_proto",
        "@googleapis//google/bytestream:bytestream_java_grpc",
        "@googleapis//google/bytestream:bytestream_java_proto",
        "@tools_remote_maven//:com_google_guava_guava",
        "@tools_remote_maven//:com_google_http_client_google_http_client",
        "@tools_remote_maven//:com_google_http_client_google_http_client_jackson2",
        "@tools_remote_maven//:com_google_jimfs_jimfs",
        "@tools_remote_maven//:com_google_protobuf_protobuf_java",
        "@tools_remote_maven//:com_google_truth_truth",
        "@tools_remote_maven//:io_grpc_grpc_api",
        "@tools_remote_maven//:io_grpc_grpc_context",
        "@tools_remote_maven//:io_grpc_grpc_core",
        "@tools_remote_maven//:io_grpc_grpc_inprocess",
        "@tools_remote_maven//:io_grpc_grpc_stub",
        "@tools_remote_maven//:io_grpc_grpc_util",
    ],
)

java_test(
    name = "ShellEscaperTest",
    srcs = ["ShellEscaperTest.java"],
    deps = [
        "//src/main/java/com/google/devtools/build/remote/client",
        "@tools_remote_maven//:com_google_truth_truth",
    ],
)

java_test(
    name = "ActionGroupingTest",
    srcs = ["ActionGroupingTest.java"],
    deps = [
        "//src/main/java/com/google/devtools/build/remote/client",
        "//src/main/proto:remote_execution_log_java_proto",
        "@bazel_remote_apis//build/bazel/remote/execution/v2:remote_execution_java_proto",
        "@googleapis//google/longrunning:longrunning_java_proto",
        "@tools_remote_maven//:com_google_protobuf_protobuf_java",
        "@tools_remote_maven//:com_google_protobuf_protobuf_java_util",
        "@tools_remote_maven//:com_google_truth_truth",
        "@tools_remote_maven//:io_grpc_grpc_api",
    ],
)

java_test(
    name = "DockerUtilTest",
    srcs = ["DockerUtilTest.java"],
    deps = [
        "//src/main/java/com/google/devtools/build/remote/client",
        "@bazel_remote_apis//build/bazel/remote/execution/v2:remote_execution_java_proto",
        "@tools_remote_maven//:com_google_guava_guava",
        "@tools_remote_maven//:com_google_truth_truth",
    ],
)
