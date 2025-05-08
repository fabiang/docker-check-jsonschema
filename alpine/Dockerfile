# syntax=docker/dockerfile:1
ARG PYTHON_VERSION=3
ARG ALPINE_VERSION=3.21
FROM python:${PYTHON_VERSION}-alpine${ALPINE_VERSION}

ARG CHECK_JSONSCHEMA_VERSION=0.33.0

RUN pip install --root-user-action=ignore check-jsonschema==${CHECK_JSONSCHEMA_VERSION}

ENTRYPOINT ["check-jsonschema"]
