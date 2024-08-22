load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "build_bazel_rules_apple",
    sha256 = "62847b3f444ce514ae386704a119ad7b29fa6dfb65a38bff4ae239f2389a0429",
    url = "https://github.com/bazelbuild/rules_apple/releases/download/3.8.0/rules_apple.3.8.0.tar.gz",
)

http_archive(
    name = "build_bazel_rules_ios",
    sha256 = "d1cc852aa9e989c12b802e04cb66dfe51418153c781d6073bb30e82284866865",
    url = "https://github.com/bazel-ios/rules_ios/releases/download/5.0.0/rules_ios.5.0.0.tar.gz",
)

load(
    "@build_bazel_rules_apple//apple:repositories.bzl",
    "apple_rules_dependencies",
)

apple_rules_dependencies()

load(
    "@build_bazel_rules_ios//rules:repositories.bzl",
    "rules_ios_dependencies"
)

rules_ios_dependencies()

load(
    "@build_bazel_rules_swift//swift:repositories.bzl",
    "swift_rules_dependencies",
)

swift_rules_dependencies()

load(
    "@build_bazel_rules_swift//swift:extras.bzl",
    "swift_rules_extra_dependencies",
)

swift_rules_extra_dependencies()

load(
    "@build_bazel_apple_support//lib:repositories.bzl",
    "apple_support_dependencies",
)

apple_support_dependencies()

load(
    "@com_google_protobuf//:protobuf_deps.bzl",
    "protobuf_deps",
)

protobuf_deps()