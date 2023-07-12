FROM --platform=linux/amd64 golang:1.20-alpine3.18
RUN apk --no-cache add tzdata  \
    gcc  \
    jq  \
    bash  \
    make  \
    coreutils \
    git \
    zlib-dev \
    zstd-libs \
    libsasl \
    lz4-dev \
    zstd-dev \
    libc-dev && \
    ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && \
    echo "Asia/Shanghai" > /etc/timezone
USER root
WORKDIR /root