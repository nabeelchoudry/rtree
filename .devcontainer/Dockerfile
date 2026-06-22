# Use a stable Ubuntu image
FROM mcr.microsoft.com/devcontainers/base:ubuntu-22.04

# Install compiler, debugger, and build tools
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends \
    build-essential \
    cmake \
    gdb \
    clang \
    libboost-dev \
    && apt-get clean && rm -rf /var/lib/apt/lists/*