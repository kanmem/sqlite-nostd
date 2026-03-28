ARG VARIANT="2-trixie"
FROM mcr.microsoft.com/devcontainers/base:${VARIANT}

RUN apt-get update && apt-get upgrade -y && apt-get install libclang-dev -y

USER vscode

RUN curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y --default-toolchain stable --profile default --component rust-analyzer
