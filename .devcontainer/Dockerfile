FROM mcr.microsoft.com/devcontainers/base:ubuntu-22.04@sha256:253b0ee40a5afd4f295640f9f90aed206953962fab56bfa14d9fcb593f33dc47

# hadolint ignore=DL3008
RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    ca-certificates \
    nodejs \
    npm \
    wget && \
    update-ca-certificates && \
    rm -rf /var/lib/apt/lists/*

ARG HUGO_VERSION="0.155.1"
RUN wget --quiet "https://github.com/gohugoio/hugo/releases/download/v${HUGO_VERSION}/hugo_extended_${HUGO_VERSION}_Linux-64bit.tar.gz" && \
    tar xzf hugo_extended_${HUGO_VERSION}_Linux-64bit.tar.gz && \
    rm -r hugo_extended_${HUGO_VERSION}_Linux-64bit.tar.gz && \
    mv hugo /usr/bin && \
    chmod 755 /usr/bin/hugo

WORKDIR /src
COPY ./ /src
