ARG PYTHON_VERSION
ARG ALPINE_VERSION

FROM python:$PYTHON_VERSION-alpine$ALPINE_VERSIONE as rjango_python-base
ENV WORK_DIR=/app
WORKDIR $WORK_DIR
RUN pip install --upgrade --no-cache-dir pip pipenv
