FROM python:3.7.4

ADD . /app

WORKDIR /app

RUN apt-get update && apt-get install -y

RUN pip3 install -r requirements.txt

EXPOSE 5000

ENV FLASK_APP=main.py

CMD ["flask", "run", "--host", "0.0.0.0"]