FROM golang:1.10-alpine

RUN apk update \
    && apk add jq \
    && rm -rf /var/cache/apk/*

ADD entrypoint.sh /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]