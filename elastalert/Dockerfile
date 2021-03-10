FROM python:alpine
LABEL maintainer="Junpei Kawamoto <junpei@storewise.tech>"
LABEL description="A docker image that provides elastalert"
LABEL org.opencontainers.image.url="https://github.com/storewise/dockerfiles/tree/master/elastalert"
LABEL org.opencontainers.image.documentation="https://github.com/storewise/dockerfiles"
LABEL org.opencontainers.image.source="https://github.com/storewise/dockerfiles"
LABEL org.opencontainers.image.vendor="StoreWise"
LABEL org.opencontainers.image.title="elastalert"
LABEL org.opencontainers.image.description="A docker image that provides elastalert"

RUN apk add --no-cache gcc musl-dev libffi-dev libressl-dev libmagic rust cargo
RUN pip install --no-cache-dir elastalert==0.2.4
