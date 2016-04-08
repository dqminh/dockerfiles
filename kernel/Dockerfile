FROM debian:jessie

RUN apt-get update && apt-get install -y \
    ca-certificates \
    curl \
    git \
    kernel-package \
    make \
    libncurses5-dev \
    libssl-dev \
    --no-install-recommends \
    && rm -rf /var/lib/apt/lists/*

ENV JOBS=4
WORKDIR /kernel
COPY config /kernel/config
COPY kernel /usr/local/bin/kernel
CMD [ "bash" ]
