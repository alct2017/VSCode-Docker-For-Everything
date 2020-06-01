FROM ubuntu

RUN sed -i 's/archive.ubuntu.com/mirrors.aliyun.com/g' /etc/apt/sources.list; \ 
    sed -i 's/security.ubuntu.com/mirrors.aliyun.com/g' /etc/apt/sources.list; \
    apt-get clean all; \
    apt-get update; \
    apt-get upgrade -y
ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get install -y build-essential gcc gdb git;