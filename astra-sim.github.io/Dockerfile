FROM ubuntu:20.04
LABEL maintainer="Taekyung Heo <tkheo@casys.kaist.ac.kr>"

ENV DEBIAN_FRONTEND=noninteractive
ENV LC_ALL="C.UTF-8"
ENV LANG="en_US.UTF-8"
ENV LANGUAGE="en_US.UTF-8"
RUN apt-get -y update \
    && apt-get -y install\
    gcc g++ make cmake\
    vim python3 ruby-dev git

RUN git clone --recurse-submodules https://github.com/astra-sim/astra-sim.github.io.git
RUN gem install bundler
