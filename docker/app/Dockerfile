FROM ubuntu:22.04

RUN apt update
RUN apt install -y python3 python3-pip vim lsof procps cron git

ENV PYTHONPATH "${PYTHONPATH}:/src"

RUN mkdir /src
WORKDIR /src
COPY requirements.txt .
RUN pip3 install -r requirements.txt
