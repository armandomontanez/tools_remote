load("@rules_java//java:java_binary.bzl", "java_binary")

java_binary(
    name = "remote_client",
    main_class = "com.google.devtools.build.remote.client.RemoteClient",
    visibility = ["//visibility:public"],
    runtime_deps = [
        "//src/main/java/com/google/devtools/build/remote/client",
    ],
)
