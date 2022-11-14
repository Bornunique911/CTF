FROM python:3.12-rc-slim
RUN useradd ctf && mkdir /app

WORKDIR /app

RUN pip3 install flask
RUN chown -R root /app
RUN umask a+rx

COPY . /app

USER ctf

EXPOSE 1337

CMD python3 app.py
