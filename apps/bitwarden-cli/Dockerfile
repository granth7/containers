FROM ghcr.io/granth7/alpine:rolling@sha256:9e9c883b650af4379c14c2202e8840a4fdb65c8c5db8302cd794af5916549a1f

ARG TARGETPLATFORM
ARG VERSION
ARG CHANNEL

LABEL org.opencontainers.image.source="https://github.com/bitwarden/clients"

WORKDIR /usr/local/bin

RUN npm i -g @bitwarden/cli@${VERSION}

COPY ./entrypoint.sh /entrypoint.sh
CMD ["/entrypoint.sh"]
