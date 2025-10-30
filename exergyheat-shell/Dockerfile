ARG BUILD_FROM
FROM $BUILD_FROM

RUN apk update && apk add --no-cache \
    bash \
    procps \
    net-tools \
    lsof \
    busybox-extras \
    curl \
    wget \
    netcat-openbsd \
    iproute2 \
    iputils \
    bind-tools \
    ttyd

CMD [ "ttyd", "--writable", "-p", "7681", "bash" ]
