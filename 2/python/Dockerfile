FROM python:3

WORKDIR /usr/src/app

COPY requirements.txt ./

RUN pip install --no-cache-dir -r requirements.txt

COPY . .

EXPOSE 8080

RUN apt update

ENTRYPOINT python app.py runserver 0.0.0.0:8080