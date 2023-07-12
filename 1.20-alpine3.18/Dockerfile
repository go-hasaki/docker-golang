FROM --platform=linux/amd64 golang:1.20-alpine3.18
RUN apk --no-cache add tzdata \
    jq \
    bash \
    make \
    coreutils && \
    ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && \
    echo "Asia/Shanghai" > /etc/timezone \
USER root
WORKDIR /root