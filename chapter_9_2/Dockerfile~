##################################################
# Dockerfile to build the unittest container

# Base image is python

FROM python:latest

# Author: hoang
MAINTAINER hoang <hoangth92.nd@gmail.com>

# install redis driver for python and redis mock

RUN pip install redis && pip install mockredispy

# Copy test an source to docker image

ADD src/ /src/

# change working directory to /src/

WORKDIR /src/

# Make unittest as default execution

ENTRYPOINT python3 -m unittest
