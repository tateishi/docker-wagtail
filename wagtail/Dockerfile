FROM python:3.11.2

RUN useradd -U ubuntu
RUN mkdir /app && chown ubuntu:ubuntu /app
USER ubuntu
WORKDIR /app
ADD requirements.txt /app/
USER root
RUN pip install -r /app/requirements.txt
USER ubuntu
