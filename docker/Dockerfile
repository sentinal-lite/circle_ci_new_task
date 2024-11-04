ARG DOCKER_PLATFORM="linux/amd64"

ARG PYTHON_VERSION="3.19"

FROM python:alpine${PYTHON_VERSION}

RUN apk update && apk upgrade 

WORKDIR /app

COPY ./src .

CMD ["python3", "app.py"]