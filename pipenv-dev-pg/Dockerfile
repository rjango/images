ARG IMAGE_BASE=rjango/pipenv-dev:2018.11.26-python3.7.3-alpine3.9

FROM $IMAGE_BASE

ARG POSTGRESQL_DEV_VERSION="11.3-r0"

RUN apk add --no-cache --virtual pg-dev-dependencies postgresql-dev=$POSTGRESQL_DEV_VERSION
