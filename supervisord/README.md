# josemrb/docker-alpine-pgweb
[![Docker Automated buil](https://img.shields.io/docker/automated/jrottenberg/ffmpeg.svg)](https://hub.docker.com/r/josemrb/docker-alpine-supervisord/)

based on docker-alpine

[supervisord 3.3.1](https://github.com/Supervisor/supervisor)


Usage
```sh
# pull image
$ docker pull josemrb/docker-alpine-pgweb

# run in a transient container
$ docker run --rm -i -t -p 8081:8081 josemrb/docker-alpine-pgweb
```
