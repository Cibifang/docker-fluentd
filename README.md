# docker-fluentd

Docker image for fluentd with support for some plugins

## Fluentd version

fluentd:v1.2-debian-onbuild

## Installed plugins

The following plugins are installed in the docker image:

1. fluent-plugin-concat

## Build

`docker build -t custom-fluentd:latest ./`

## Ports

| Port   | Description      |
|--------|------------------|
| 24224  | Forward Protocol |

## Run

`docker run -d -p 24224:24224 -p 24224:24224/udp -v /data:/fluentd/log custom-fluentd:latest`
