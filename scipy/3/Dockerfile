FROM giodegas/pypy-jupyter:3

MAINTAINER G De Gasperis <giovanni@giodegas.it>

RUN apt-get update && apt-get upgrade -q -y && \
    apt-get install -q -y gfortran

RUN pip install --upgrade pip
RUN pip install scipy ipython jupyter pandas sympy pytest nose Pillow GMM
RUN pip install --pre scikit-learn
COPY compat.py /usr/local/site-packages/sklearn/externals/joblib/externals/loky/backend/.

EXPOSE 8888/tcp
