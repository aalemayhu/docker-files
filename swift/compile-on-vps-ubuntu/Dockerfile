FROM ubuntu:14:04
MAINTAINER Alexander Alemayhu <alexander@alemayhu.com>

# Packages needed
RUN apt-get update && \
apt-get install git cmake ninja-build clang python uuid-dev libicu-dev \
icu-devtools libbsd-dev libedit-dev libxml2-dev libsqlite3-dev swig \
libpython-dev libncurses5-dev pkg-config -y

# Source code
RUN git clone https://github.com/apple/swift
RUN git clone https://github.com/ninja-build/ninja.git
RUN cd swift && utils/update-checkout --clone

RUN time utils/build-script -t
