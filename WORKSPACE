load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

RULES_COBOL_VERSION = "0.1.0"

http_archive(
    name = "io_bazel_rules_cobol",
    sha256 = "465d6185382baf98ee1273efa4ff0f26e47524b2f6954b7b8071c5b48d21932e",
    strip_prefix = "rules_cobol-{v}".format(v = RULES_COBOL_VERSION),
    urls = [
        "https://github.com/Fuwn/rules_cobol/archive/refs/tags/{v}.zip".format(v = RULES_COBOL_VERSION),
    ],
)

load("@io_bazel_rules_cobol//cobol:deps.bzl", "cobol_rules_dependencies")

cobol_rules_dependencies()
