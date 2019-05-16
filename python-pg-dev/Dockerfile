ARG PYTHON_VERSION=3.7.3
ARG ALPINE_VERSION=3.9

FROM registry.gitlab.com/rjango/images/python-dev:$PYTHON_VERSION-alpine$ALPINE_VERSION

RUN apk add --no-cache --virtual pg-dev-dependencies postgresql-dev
