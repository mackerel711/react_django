FROM python:3.7
ENV PYTHONUNBUFFERED 1
RUN mkdir /code
WORKDIR /code
ADD requirements.txt /code/
RUN apt update
RUN apt install nginx
RUN pip3 install -r requirements.txt
ADD . /code/
EXPOSE 9002