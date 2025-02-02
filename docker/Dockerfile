FROM node:alpine3.20

ARG ROOT=/RisuAI

WORKDIR ${ROOT}

RUN apk add git && \
    git clone https://github.com/kwaroran/RisuAI.git . && \
    npm i -g pnpm && pnpm install && pnpm run build

ENTRYPOINT [ "/bin/sh", "-c", "pnpm run runserver" ]
