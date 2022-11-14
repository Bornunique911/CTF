FROM python:3.12-rc-slim

ADD . /app

WORKDIR /app

RUN pip3 install -r requirements.txt

CMD [ "python3", "waf.py"]