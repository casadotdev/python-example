FROM nvidia/driver:418.40.04-ubuntu18.04

RUN apt-get -y update \
    && apt-get install -y software-properties-common \
    && apt-get -y update \
    && add-apt-repository universe

COPY /root/ /root
WORKDIR /root

RUN apt-get -y update \
    && apt-get -y install python3 python3-pip \
    && pip3 install --upgrade pip \
    && pip3 install -r requirements.txt
