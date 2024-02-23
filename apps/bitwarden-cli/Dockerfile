FROM node:21.6-bookworm as build

ARG BW_VERSION=2024.1.0

LABEL org.opencontainers.image.source="https://github.com/bitwarden/clients"

WORKDIR /usr/local/bin

RUN npm i -g @bitwarden/cli@${BW_VERSION}

COPY ./entrypoint.sh /entrypoint.sh
CMD ["/entrypoint.sh"]
