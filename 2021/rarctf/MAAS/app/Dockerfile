FROM python:3.12-rc-slim-buster
WORKDIR /app
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt
COPY static static
COPY templates templates
EXPOSE 5000
COPY app.py app.py
ENTRYPOINT ["python", "app.py"]
