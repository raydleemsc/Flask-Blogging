FROM python:3.11.10-slim-bullseye
ENV PYTHONUNBUFFERED 1
RUN mkdir /app
WORKDIR /app
ADD docker-requirements.txt /app/
RUN apt-get update
RUN apt-get install sqlite3
RUN pip install -r docker-requirements.txt
ADD . /app/