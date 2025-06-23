FROM mcr.microsoft.com/devcontainers/base:ubuntu

# Install Rust
RUN apt-get update && \
    apt-get install -y curl build-essential pkg-config libssl-dev && \
    curl https://sh.rustup.rs -sSf | sh -s -- -y && \
    chmod -R a+w $HOME/.cargo

ENV PATH="/root/.cargo/bin:${PATH}"
