FROM python:3.9

RUN apt-get update && \
  apt-get upgrade -y

RUN pip install --upgrade pip && \
  pip install poetry

WORKDIR /app
COPY pyproject.toml poetry.lock ./
RUN poetry install
