FROM pypy:3

MAINTAINER G De Gasperis <giovanni@giodegas.it>

RUN apt-get update && apt-get install -q -y apt-utils && apt-get upgrade -q -y
RUN apt-get install -q -y build-essential autogen autoconf automake git \
                          vim nano \
                          libcurl4-openssl-dev libgmp-dev libjansson-dev libblas-dev liblapack-dev

RUN pip install --upgrade pip
RUN pip install requests selenium numpy matplotlib jupyter pytest
COPY dotest /

EXPOSE 8888/tcp

