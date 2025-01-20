FROM public.ecr.aws/docker/library/python:3.10-alpine

WORKDIR /src

COPY analytics/requirements.txt requirements.txt 

RUN pip install -r requirements.txt 

COPY analytics/app.py app.py

COPY analytics/config.py config.py

CMD ["/bin/sh", "-c", "python app.py"]
