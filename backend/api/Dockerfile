FROM python:3.11-slim
ENV POETRY_VIRTUALENVS_CREATE=false

RUN pip install poetry

COPY . /api
WORKDIR /api

RUN poetry config installer.max-workers 10
RUN poetry install --no-interaction --no-ansi

