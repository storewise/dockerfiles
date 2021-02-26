FROM python:alpine
LABEL maintainer="Junpei Kawamoto <junpei@storewise.tech>"
LABEL description="A docker image that provides curator"

RUN pip install --no-cache-dir elasticsearch-curator==5.8.3
ENTRYPOINT ["curator"]
