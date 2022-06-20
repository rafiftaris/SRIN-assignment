# pull official base image
FROM python:3.11-rc-slim

# set work directory
WORKDIR /usr/src/app

# set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# install dependencies requirements
RUN apt-get update && apt-get -y upgrade

# install dependencies
RUN pip install --upgrade pip

# copy project
COPY . /usr/src/app/

# expose to port 8080
EXPOSE 8000