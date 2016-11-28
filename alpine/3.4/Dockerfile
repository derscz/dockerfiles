FROM alpine:3.4

MAINTAINER Milan Sulc <sulc@ders.cz>

ENV TERM xterm
ENV USER_UID 1000
ENV USER_NAME ders

RUN apk update && \
    apk upgrade && \
    adduser -D -u $USER_UID $USER_NAME && \
    rm -rf /var/cache/apk/*

CMD ["/bin/sh"]
