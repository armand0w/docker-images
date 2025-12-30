FROM debian@sha256:c71b05eac0b20adb4cdcc9f7b052227efd7da381ad10bb92f972e8eae7c6cdc9

LABEL maintainer="Armando Castillo H"

ENV JAVA_HOME=/usr/bin/java
ENV PATH=$JAVA_HOME/bin:$PATH

RUN apt-get update \
    && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
        openjdk-21-jre-headless \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
