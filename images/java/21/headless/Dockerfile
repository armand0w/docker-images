FROM debian@sha256:88ef4df0f82963ff3c0472493da188f082822b2a16b1be23d238d124d5c8c92e

LABEL maintainer="Armando Castillo H"

ENV JAVA_HOME=/usr/bin/java
ENV PATH=$JAVA_HOME/bin:$PATH

RUN apt-get update \
    && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
        openjdk-21-jre-headless \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
