FROM python:3.12-rc-slim
RUN pip3 --no-cache-dir install flask gunicorn
WORKDIR /srv
COPY jar.py pickle.jpg ./
ENV FLAG="actf{REDACTED}"
EXPOSE 5000
USER nobody
CMD python jar.py