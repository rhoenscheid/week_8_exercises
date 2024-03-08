FROM mcr.microsoft.com/devcontainers/cpp:0-ubuntu-22.04

RUN apt-get update \
        && export DEBIAN_FRONTEND=noninteractive \
        && apt-get -y install --no-install-recommends valgrind clang-format openmpi-bin libopenmpi-dev gnuplot \
        && apt-get autoremove -y \
        && apt-get clean -y \
        && rm -rf /var/lib/apt/lists/*

ENV LD_LIBRARY_PATH=/usr/local/lib/:$LD_LIBRARY_PATH