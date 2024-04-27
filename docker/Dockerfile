FROM alpine
RUN mkdir /app
COPY train.py /app
COPY predict.py /app
RUN apk add \
    wget \
    gcc \
    make \
    zlib-dev \
    libffi-dev \
    openssl-dev \
    musl-dev


ENV PYTHONUNBUFFERED=1
RUN apk add --update --no-cache python3 && ln -sf python3 /usr/bin/python
#RUN python3 -m ensurepip
#RUN pip3 install --no-cache --upgrade pip setuptools

RUN echo "http://dl-8.alpinelinux.org/alpine/edge/community" >> /etc/apk/repositories
#RUN apk --no-cache --update-cache add gcc gfortran python python-dev py-pip build-base wget freetype-dev libpng-dev openblas-dev
RUN ln -s /usr/include/locale.h /usr/include/xlocale.h
#RUN pip install numpy scipy pandas matplotlib
#RUN pip install --no-cache-dir numpy scipy pandas matplotlib
RUN apk add --update py-pip
RUN apk add py3-setuptools
RUN pip install --no-cache-dir numpy
