FROM ubuntu:16.04
LABEL maintainer="glitchylabs@gmail.com"

WORKDIR /app/

RUN apt-get update -qy \
    && apt-get install -qy cmake build-essential libboost-all-dev git ca-certificates --no-install-recommends \
    && apt-get install automake autoconf pkg-config libcurl4-openssl-dev libjansson-dev libssl-dev libgmp-dev make g++
