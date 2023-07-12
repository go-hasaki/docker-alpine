FROM --platform=linux/amd64 alpine:3.18
RUN echo "https://mirrors.aliyun.com/alpine/v3.18/main/" > /etc/apk/repositories
RUN echo "https://mirrors.aliyun.com/alpine/v3.18/community/" >> /etc/apk/repositories
RUN apk update
RUN apk --no-cache add ca-certificates
RUN apk --no-cache add tzdata  && \
    ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && \
    echo "Asia/Shanghai" > /etc/timezone