FROM python:3.8-slim-buster

COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt
COPY . ./application
WORKDIR /application
CMD gunicorn --bind 0.0.0.0:$PORT wsgi