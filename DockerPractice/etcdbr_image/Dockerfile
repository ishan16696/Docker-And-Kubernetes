FROM alpine:3.10.1

RUN apk add --update bash curl

COPY etcdbrctl /usr/local/bin/etcdbrctl
WORKDIR /
COPY 00-backup-restore-server-config.yaml /
ENTRYPOINT ["/usr/local/bin/etcdbrctl", "server","--config-file=/00-backup-restore-server-config.yaml"]

