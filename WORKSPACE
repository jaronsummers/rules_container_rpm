load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive", "http_file")

http_archive(
    name = "io_bazel_rules_docker",
    sha256 = "4521794f0fba2e20f3bf15846ab5e01d5332e587e9ce81629c7f96c793bb7036",
    strip_prefix = "rules_docker-0.14.4",
    urls = ["https://github.com/bazelbuild/rules_docker/archive/v0.14.4.tar.gz"],
)

load(
    "@io_bazel_rules_docker//repositories:repositories.bzl",
    container_repositories = "repositories",
)

container_repositories()

http_file(
    name = "glibc",
    sha256 = "573ceb6ad74b919b06bddd7684a29ef75bc9f3741e067fac1414e05c0087d0b6",
    urls = ["https://dl.fedoraproject.org/pub/fedora/linux/releases/28/Everything/x86_64/os/Packages/g/glibc-2.27-8.fc28.x86_64.rpm"],
)

http_file(
    name = "ca_certificates",
    sha256 = "dfc3d2bf605fbea7db7f018af53fe0563628f788a40cb1e7f84434606b7b6a12",
    urls = ["https://dl.fedoraproject.org/pub/fedora/linux/releases/28/Everything/x86_64/os/Packages/c/ca-certificates-2018.2.22-3.fc28.noarch.rpm"],
)
