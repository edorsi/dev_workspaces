FROM mcr.microsoft.com/devcontainers/rust:1-1-bullseye

# Install generic tools + gRPC/Protobuf compiler
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends \
    postgresql-client \
    iputils-ping \
    protobuf-compiler \
    libprotobuf-dev

# Pre-install global Cargo tools (optional)
RUN cargo install cargo-expand cargo-edit
