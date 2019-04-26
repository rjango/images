ARG PYTHON_VERSION
ARG ALPINE_VERSION

FROM python:$PYTHON_VERSION-alpine$ALPINE_VERSIONE

ENV WORK_DIR=/app VENV_DIR=/venv PATH=$VENV_DIR/bin:$PATH

WORKDIR $WORK_DIR

RUN mkdir -p $WORK_DIR && python3 -m venv $VENV_DIR && pip install --upgrade --no-cache-dir pip pipenv
