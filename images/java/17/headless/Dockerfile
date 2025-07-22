FROM debian@sha256:b6507e340c43553136f5078284c8c68d86ec8262b1724dde73c325e8d3dcdeba

LABEL maintainer="Armando Castillo H"

ENV JAVA_HOME=/usr/bin/java
ENV PATH=$JAVA_HOME/bin:$PATH

RUN apt-get update \
    && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
        openjdk-17-jre-headless \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
