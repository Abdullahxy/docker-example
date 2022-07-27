FROM python:3.8-alpine3.11

# update apk repo
RUN echo "http://dl-4.alpinelinux.org/alpine/v3.11/main" >> /etc/apk/repositories && \
    echo "http://dl-4.alpinelinux.org/alpine/v3.11/community" >> /etc/apk/repositories

# install chromedriver
RUN apk --no-cache add chromium-chromedriver

# upgrading pip and cffi
RUN /usr/local/bin/python -m pip install --upgrade pip
RUN pip install --upgrade cffi

# install selenium
RUN pip install selenium
