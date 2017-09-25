FROM gocd/gocd-agent-alpine-3.5:v17.10.0

# Installs NodeJS and Node-Gyp dependencies
RUN apk update && \
    apk add --update --no-cache \
    nodejs bash python make g++ && \
    rm -rf /var/cache/apk/*
