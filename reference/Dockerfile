FROM tensorflow/tensorflow:1.1.0-rc0-gpu

LABEL author="yaoyuan7 <yaoyuan0608@gmail.com>"

RUN apt-get update && apt-get install -y  \
    autoconf \
    automake \
    bzip2 \
    g++ \
    git \
    gstreamer1.0-plugins-good \
    gstreamer1.0-tools \
    gstreamer1.0-pulseaudio \
    gstreamer1.0-plugins-bad \
    gstreamer1.0-plugins-base \
    gstreamer1.0-plugins-ugly  \
    libatlas3-base \
    libgstreamer1.0-dev \
    libtool-bin \
    make \
    python2.7 \
    python-pip \
    python-yaml \
    python-simplejson \
    python-gi \
    subversion \
    wget \
    zlib1g-dev && \
    apt-get clean autoclean && \
    apt-get autoremove -y && \
    pip install ws4py==0.3.2 && \
    pip install tornado && \    
    ln -s /usr/bin/python2.7 /usr/bin/python ; ln -s -f bash /bin/sh


ENV LD_LIBRARY_PATH /usr/local/nvidia${LD_LIBRARY_PATH:+:${LD_LIBRARY_PATH}}

ENV PATH /usr/local/cuda-8.0/targets/x86_64-linux/lib/stubs${PATH:+:${PATH}}

ENV LD_LIBRARY_PATH /usr/local/nvidia${LD_LIBRARY_PATH:+:${LD_LIBRARY_PATH}}

ENV LD_LIBRARY_PATH /usr/local/cuda-8.0/targets/x86_64-linux/lib/stubs${LD_LIBRARY_PATH:+:${LD_LIBRARY_PATH}}
