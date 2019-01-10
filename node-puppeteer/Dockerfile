FROM node:10-alpine

ENV CHROME_BIN="/usr/bin/chromium-browser" \
    PUPPETEER_SKIP_CHROMIUM_DOWNLOAD="true"
    
RUN apk update \
    && apk add jq \
        chromium  \
    && rm -rf /var/cache/apk/*

ADD entrypoint.sh /entrypoint.sh

ENTRYPOINT [ "/entrypoint.sh" ]