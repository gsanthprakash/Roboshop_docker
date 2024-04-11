FROM python:3.9

EXPOSE 8080

USER root

WORKDIR /app
COPY requirements.txt /app/
RUN pip install -r requirements.txt
COPY *.py /app/
COPY payment.ini

CMD ["uwsgi", "--ini", "payment.ini"]