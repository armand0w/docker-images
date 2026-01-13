FROM debian@sha256:5cf544fad978371b3df255b61e209b373583cb88b733475c86e49faa15ac2104

LABEL maintainer="Armando Castillo H"

ENV JAVA_HOME=/usr/bin/java
ENV PATH=$JAVA_HOME/bin:$PATH

RUN apt-get update \
    && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
        openjdk-17-jre-headless \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
