FROM mcr.microsoft.com/devcontainers/base:ubuntu

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends \
        build-essential cmake gdb pkg-config \
        qt6-base-dev qt6-tools-dev qt6-tools-dev-tools \
        xorg xvfb x11-utils fonts-noto-cjk \
    && apt-get clean && rm -rf /var/lib/apt/lists/*

ENV DISPLAY=:99
