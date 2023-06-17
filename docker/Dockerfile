FROM node:19.1.0-alpine3.16

ARG ROOT=/RisuAI

WORKDIR ${ROOT}

RUN apk add git && \
    git clone https://github.com/kwaroran/RisuAI.git . && \
    npm i && npm run build

ENTRYPOINT [ "/bin/sh", "-c", "npm run runserver" ]