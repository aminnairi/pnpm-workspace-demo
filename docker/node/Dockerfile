FROM node:18.0.0-alpine

ENV PNPM_HOME="/home/node/.local/share/pnpm"
ENV PATH="$PNPM_HOME:$PATH"

USER node

WORKDIR /home/node

RUN wget -q https://get.pnpm.io/install.sh

RUN PNPM_VERSION=8.1.1 ENV="$HOME/.shrc" SHELL="$(which sh)" sh install.sh

RUN pnpm --version
