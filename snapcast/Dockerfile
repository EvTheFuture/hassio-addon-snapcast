ARG BUILD_FROM
FROM $BUILD_FROM

ENV LANG C.UTF-8

SHELL ["/bin/bash", "-o", "pipefail", "-c"]

# Copy data for add-on
COPY rootfs /

RUN printf "@edge http://dl-cdn.alpinelinux.org/alpine/edge/main\n@edge http://dl-cdn.alpinelinux.org/alpine/edge/community\n@edge http://dl-cdn.alpinelinux.org/alpine/edge/testing\n" >> /etc/apk/repositories  
RUN apk update
RUN apk add --no-cache openrc
RUN apk add --no-cache snapcast@edge snapcast-server@edge snapcast-client@edge
RUN apk add --no-cache librespot@edge
RUN apk add --no-cache alsa-plugins-pulse
#RUN apk add --no-cache neovim screen

