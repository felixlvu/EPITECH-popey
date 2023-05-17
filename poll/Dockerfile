FROM python:3

WORKDIR /app

ENV FLASK_ENV docker
ENV FLASK_APP app.py

COPY requirements.txt /app
RUN pip3 install -r requirements.txt

EXPOSE 80

COPY . /app

CMD ["flask", "run", "--host=0.0.0.0", "--port=80"]
