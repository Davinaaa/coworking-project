FROM python:3.10-slim-buster

WORKDIR /src

COPY ./requirements.txt requirements.txt 

RUN pip install -r requirements.txt 

COPY ./app.py app.py

COPY ./config.py config.py

CMD python app.py