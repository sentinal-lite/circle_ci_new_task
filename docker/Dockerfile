ARG DOCKER_PLATFORM="linux/amd64"

ARG PYTHON_VERSION="3.19"

FROM python:alpine${PYTHON_VERSION}

RUN apk update && apk upgrade 

WORKDIR /app

COPY requirements.txt requirements.txt

RUN pip install -r requirements.txt

COPY ./src .

RUN rm requirements.txt

CMD ["python3", "app.py"]