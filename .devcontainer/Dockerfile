FROM ubuntu:22.04

# Install build essentials and cmake
RUN apt-get update && apt-get install -y \
    build-essential \
    cmake \
    gdb \
    git \
    && rm -rf /var/lib/apt/lists/*

# Create non-root user for VS Code
RUN useradd -ms /bin/bash vscode
USER vscode
WORKDIR /workspace
