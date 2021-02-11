#############################################################
# A docker with the prerequisites libraries to run SpyGlass #
#############################################################
FROM ubuntu:18.04

MAINTAINER m4j0rt0m

# install prerequisite software
RUN apt-get update && \
    DEBIAN_FRONTEND=noninteractive apt-get install -y \
    git make autoconf g++ flex bison file \
    gperf libreadline6-dev libncurses5-dev \
    libglib2.0-0 libsm6 libfontconfig1 libxrender1 && \
    apt-get clean

# force the use of bash
RUN ln -sf /bin/bash /bin/sh

WORKDIR /root
