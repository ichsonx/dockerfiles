# 作为开发、测试用的ubunt18镜像
FROM ubuntu:latest
# 原因是在使用apt-get安装依赖时，可能会有对话框，制作镜像时如果不选择会导致失败，因此加入这句
ENV DEBIAN_FRONTEND noninteractive
# 安装systemd后，就可以在 Dockerfile 或者 docker run 命令中使用 sleep infinity,容器就不会因没有前台常驻线程而刚启动就结束退出
RUN apt-get update && apt-get install -y curl net-tools vim systemd wget lrzsz git gcc cmake docker.io zip bridge-utils
CMD ["/bin/sh" "-c" "sleep infinity"]