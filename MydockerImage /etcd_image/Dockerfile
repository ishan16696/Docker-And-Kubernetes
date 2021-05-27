FROM alpine:3.10.1

RUN apk add --update bash curl

COPY etcd /usr/local/bin/etcd
WORKDIR /
ENTRYPOINT ["/usr/local/bin/etcd","--data-dir=default.etcd","--listen-client-urls=http://0.0.0.0:2379","--advertise-client-urls=http://0.0.0.0:2379"]
