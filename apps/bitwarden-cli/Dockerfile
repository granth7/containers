FROM node:21.6-bookworm as build

ARG VERSION

LABEL org.opencontainers.image.source="https://github.com/bitwarden/clients"

WORKDIR /usr/local/bin

RUN npm i -g @bitwarden/cli@${VERSION}

COPY ./apps/bitwarden-cli/entrypoint.sh /entrypoint.sh
CMD ["/entrypoint.sh"]
