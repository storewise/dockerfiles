FROM python:3.8
LABEL maintainer="Junpei Kawamoto <junpei@storewise.tech>"
LABEL description="A docker image that provides curator"
LABEL org.opencontainers.image.url="https://github.com/storewise/dockerfiles/tree/master/curator"
LABEL org.opencontainers.image.documentation="https://github.com/storewise/dockerfiles"
LABEL org.opencontainers.image.source="https://github.com/storewise/dockerfiles"
LABEL org.opencontainers.image.vendor="StoreWise"
LABEL org.opencontainers.image.title="curator"
LABEL org.opencontainers.image.description="A docker image that provides curator"

RUN pip install --no-cache-dir elasticsearch-curator==5.8.2
ENTRYPOINT ["curator"]
