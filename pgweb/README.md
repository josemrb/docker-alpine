# josemrb/alpine-pgweb
[![Docker Automated build](https://img.shields.io/docker/automated/jrottenberg/ffmpeg.svg)](https://hub.docker.com/r/josemrb/alpine-pgweb/)

based on [josemrb/alpine-supervisord](https://hub.docker.com/r/josemrb/alpine-supervisord/)

[pgweb 0.9.5](https://github.com/sosedoff/pgweb)

Usage

```sh
# pull image
$ docker pull josemrb/alpine-pgweb

# run in a transient container
$ docker run --rm -i -t -p 8081:8081 josemrb/alpine-pgweb
```
