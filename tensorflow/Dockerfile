FROM pypy:3-7

MAINTAINER Aly Shmahell <aly.shmahell@gmail.com>

RUN apt-get update && apt-get install -q -y apt-utils && apt-get upgrade -q -y
RUN apt-get install -q -y build-essential autogen autoconf automake git \
                          vim nano \
                          libcurl4-openssl-dev libgmp-dev libjansson-dev libblas-dev liblapack-dev \
                          libpng-dev libfreetype6-dev pkg-config

RUN pip install --upgrade pip
RUN pip install --upgrade setuptools
RUN pip install cycler python-dateutil kiwisolver pyparsing requests selenium numpy matplotlib jupyter pytest tensorflow
COPY dotest /

EXPOSE 8888/tcp

