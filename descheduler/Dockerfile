FROM k8s.gcr.io/descheduler/descheduler:v0.18.0
RUN echo "http://mirrors.aliyun.com/alpine/v3.11/main" > /etc/apk/repositories \
&& apk add --no-cache curl tzdata bash\
&& cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
&& echo "Asia/Shanghai" > /etc/timezone \
&& apk del tzdata \
&& rm -rf /var/cache/apk/* \
&& rm -rf /root/.cache \
&& rm -rf /tmp/*
MAINTAINER zhengmingyi <17733101396@163.com>
