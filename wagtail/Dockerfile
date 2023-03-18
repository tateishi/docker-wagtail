FROM python:3.11.2

RUN useradd -U ubuntu
RUN mkdir /app && chown ubuntu:ubuntu /app

ADD requirements.txt /tmp/
RUN pip install -r /tmp/requirements.txt

USER ubuntu
WORKDIR /app
