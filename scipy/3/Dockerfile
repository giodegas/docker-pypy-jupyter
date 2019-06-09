FROM giodegas/pypy-jupyter:3dev

MAINTAINER G De Gasperis <giovanni@giodegas.it>

RUN apt-get update && apt-get upgrade -q -y && \
    apt-get install -q -y gfortran

RUN pip3 install --upgrade pip
RUN pip3 install Cython scipy ipython jupyter pandas sympy Pillow GMM 
RUN pip3 install scikit-learn scikit-image gensim

EXPOSE 8888/tcp
