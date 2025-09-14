FROM python:3.9
EXPOSE 8080       #{it is just documentation purpose.it tell them it is opening is port number 8080}
WORKDIR /opt/server
COPY *.py .
COPY payment.ini .
COPY requirements.txt .
RUN pip3 install -r requirements.txt
CMD ["uwsgi","--ini","payment.ini"]