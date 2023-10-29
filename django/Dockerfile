FROM python:3.9.11
ENV PYTHONUNBUFFERED 1
WORKDIR /django
ADD requirements.txt /django/
RUN pip install -r requirements.txt
ADD . /django/

