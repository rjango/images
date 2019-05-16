ARG PYTHON_VERSION
ARG ALPINE_VERSION

FROM python:$PYTHON_VERSION-alpine$ALPINE_VERSIONE as rjango_python-base
ENV WORK_DIR=/app VENV_DIR=/venv
RUN mkdir -p $WORK_DIR && pip install --upgrade --no-cache-dir pip pipenv
WORKDIR $WORK_DIR
