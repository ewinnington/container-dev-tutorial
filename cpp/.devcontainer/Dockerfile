# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.148.1/containers/cpp/.devcontainer/base.Dockerfile

# [Choice] Debian / Ubuntu version: debian-10, debian-9, ubuntu-20.04, ubuntu-18.04
ARG VARIANT="buster"
FROM mcr.microsoft.com/vscode/devcontainers/cpp:0-${VARIANT}

# [Optional] Uncomment this section to install additional packages.
RUN apt-get update -o Acquire::Check-Valid-Until=false -o Acquire::Check-Date=false && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends build-essential tar curl zip unzip cmake pkg-config

RUN git clone https://github.com/microsoft/vcpkg && ./vcpkg/bootstrap-vcpkg.sh && ./vcpkg/vcpkg update && ./vcpkg/vcpkg install sqlite3 amqpcpp boost-asio cpp-redis cpprestsdk