FROM giodegas/pypy-jupyter:3dev

MAINTAINER G De Gasperis <giovanni@giodegas.it>

RUN apt-get update && apt-get upgrade -q -y && \
    apt-get install -q -y gfortran

RUN pip install --upgrade pip
RUN pip install scipy ipython jupyter pandas sympy Pillow GMM 
RUN pip install scikit-learn
# COPY compat.py /usr/local/site-packages/sklearn/externals/joblib/externals/loky/backend/.
RUN pip install Cython 
RUN pip install scikit-image gensim

EXPOSE 8888/tcp
