ARG VARIANT="alpine-3.22"
FROM mcr.microsoft.com/devcontainers/base:${VARIANT}

RUN apk update && apk upgrade

USER vscode

RUN curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y --default-toolchain stable --profile default --component rust-analyzer
