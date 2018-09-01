FROM pypy-jupyter:3

MAINTAINER G De Gasperis <giovanni@giodegas.it>

RUN apt-get update && apt-get upgrade -q -y && \
    apt-get install -q -y lapack

RUN pip install --upgrade pip
RUN pip install scipy

EXPOSE 8888/tcp
