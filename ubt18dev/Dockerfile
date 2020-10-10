# 作为开发、测试用的ubunt18镜像
FROM ubuntu:latest
# 原因是在使用apt-get安装依赖时，可能会有对话框，制作镜像时如果不选择会导致失败，因此加入这句
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update && apt-get install -y curl net-tools vim systemd wget lrzsz git gcc cmake docker.io zip bridge-utils