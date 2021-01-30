FROM ubuntu:18.04

RUN apt-get update

RUN apt-get install -y apt-utils

RUN apt-get install -y build-essential \
  clang \
  cmake \
  git \
  net-tools \
  ruby \
  vim \
  wget \
  zsh

RUN apt-get install -y curl

RUN apt-get install -y python3 python-pip python3-pip

RUN apt-get install -y flex bison gperf python-setuptools ninja-build ccache libffi-dev libssl-dev dfu-util

RUN apt-get install -y geany
RUN apt-get -y install meld
RUN apt-get install -y gnome-icon-theme
RUN apt-get install -y dbus-x11

COPY .zshrc /root
COPY .vimrc /root

ENV DISPLAY=:0.0

WORKDIR /WORK

CMD ["/bin/zsh"]

