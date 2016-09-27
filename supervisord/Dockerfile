FROM alpine:3.4
MAINTAINER Jose Miguel Rivero Bruno <work@josemrb.com>

ENV PYTHON_VERSION=2.7.12-r0
ENV PY_PIP_VERSION=8.1.2-r0
ENV SUPERVISORD_VERSION=3.3.1

RUN \
  apk update && \
  apk add -u ca-certificates && \
  apk add -u python=$PYTHON_VERSION py-pip=$PY_PIP_VERSION

RUN update-ca-certificates

RUN pip install supervisor==$SUPERVISORD_VERSION

COPY supervisord.conf /etc/supervisor/supervisord.conf

EXPOSE 9001

ENTRYPOINT ["/usr/bin/supervisord"]
CMD ["-c", "/etc/supervisor/supervisord.conf"]
