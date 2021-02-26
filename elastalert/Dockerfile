FROM python:alpine
LABEL maintainer="Junpei Kawamoto <junpei@storewise.tech>"
LABEL description="A docker image that provides elastalert"

RUN apk add --no-cache gcc musl-dev libffi-dev libressl-dev libmagic rust cargo
RUN pip install --no-cache-dir elastalert==0.2.4
