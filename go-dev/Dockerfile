FROM ubuntu:latest

RUN apt-get update

RUN apt-get install -y curl vim git

RUN curl -O curl -O https://dl.google.com/go/go1.12.linux-amd64.tar.gz && \
    tar -C /usr/local -xzf go1.12.linux-amd64.tar.gz && \
    echo "export PATH=$PATH:/usr/local/go/bin" > ~/.bashrc

RUN mkdir -p /go/src

WORKDIR /go/src

ENTRYPOINT /bin/bash

