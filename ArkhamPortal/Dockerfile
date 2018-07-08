FROM python:2.7-slim
MAINTAINER Harsh Tyagi <23ht11tyagi@gmail.com>

ENV INSTALL_PATH /Portal
RUN mkdir -p $INSTALL_PATH

WORKDIR $INSTALL_PATH

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

COPY . .
RUN pip install --editable .

CMD gunicorn -b 0.0.0.0:8000 --access-logfile - "Portal.app:create_app()"