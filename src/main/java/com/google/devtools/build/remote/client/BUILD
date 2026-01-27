licenses(["notice"])  # Apache 2.0

load("@rules_java//java:java_library.bzl", "java_library")

java_library(
    name = "client",
    srcs = glob(["*.java"]),
    visibility = ["//:__subpackages__"],
    runtime_deps = [
        # Needed for tls client.
        "@tools_remote_maven//:io_netty_netty_tcnative_boringssl_static",
    ],
    deps = [
        "//src/main/proto:remote_execution_log_java_proto",
        "//third_party/remote-apis:build_bazel_remote_execution_v2_remote_execution_java_grpc",
        "@protobuf//:protobuf_java",
        "@protobuf//:protobuf_java_util",
        "@googleapis//google/bytestream:bytestream_java_grpc",
        "@googleapis//google/bytestream:bytestream_java_proto",
        "@googleapis//google/longrunning:longrunning_java_proto",
        "@tools_remote_maven//:com_beust_jcommander",
        "@tools_remote_maven//:com_google_auth_google_auth_library_credentials",
        "@tools_remote_maven//:com_google_auth_google_auth_library_oauth2_http",
        "@tools_remote_maven//:com_google_code_findbugs_jsr305",
        "@tools_remote_maven//:com_google_guava_guava",
        "@tools_remote_maven//:com_googlecode_json_simple_json_simple",
        "@tools_remote_maven//:io_grpc_grpc_api",
        "@tools_remote_maven//:io_grpc_grpc_auth",
        "@tools_remote_maven//:io_grpc_grpc_context",
        "@tools_remote_maven//:io_grpc_grpc_core",
        "@tools_remote_maven//:io_grpc_grpc_netty",
        "@tools_remote_maven//:io_grpc_grpc_protobuf",
        "@tools_remote_maven//:io_grpc_grpc_stub",
        "@tools_remote_maven//:io_netty_netty_handler",
        "@bazel_remote_apis//build/bazel/remote/execution/v2:remote_execution_java_proto",
        "@bazel_remote_apis//build/bazel/semver:semver_java_proto",
    ],
)
