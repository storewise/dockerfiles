FROM curlimages/curl:7.75.0
LABEL maintainer="Junpei Kawamoto <junpei@storewise.tech>"
LABEL description="A docker image that provides jq with curl"
LABEL org.opencontainers.image.url="https://github.com/storewise/dockerfiles/tree/master/jq"
LABEL org.opencontainers.image.documentation="https://github.com/storewise/dockerfiles"
LABEL org.opencontainers.image.source="https://github.com/storewise/dockerfiles"
LABEL org.opencontainers.image.vendor="StoreWise"
LABEL org.opencontainers.image.title="jq with curl"
LABEL org.opencontainers.image.description="A docker image that provides jq with curl"

USER root
RUN apk add --no-cache jq=1.6-r1

USER curl_user
ENTRYPOINT ["/bin/sh"]
