FROM debian:latest as build

COPY docker-entrypoint.sh /usr/local/bin
COPY bgpalerter-linux-x64 /

RUN mkdir /alertdata

RUN chmod +x /bgpalerter-linux-x64

# For docker only
ENTRYPOINT ["/bin/sh", "/usr/local/bin/docker-entrypoint.sh"]

