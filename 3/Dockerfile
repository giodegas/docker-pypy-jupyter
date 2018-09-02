FROM pypy:3

MAINTAINER G De Gasperis <giovanni@giodegas.it>

RUN apt-get update && apt-get upgrade -q -y && \
    apt-get install -q -y build-essential autogen autoconf automake git \
                          vim nano \
                          libcurl4-openssl-dev libgmp-dev libjansson-dev libblas-dev liblapack-dev

RUN pip install --upgrade pip
RUN pip install numpy matplotlib jupyter 

EXPOSE 8888/tcp

