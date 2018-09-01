FROM pypy:2

MAINTAINER G De Gasperis <giovanni@giodegas.it>

RUN apt-get update && apt-get upgrade -q -y && \
    apt-get install -q -y build-essential autogen autoconf automake git libcurl4-openssl-dev libgmp-dev libjansson-dev

RUN pip install --upgrade pip
RUN pip install numpy scipy jupyter

EXPOSE 8888/tcp
