FROM curlimages/curl:7.75.0
LABEL maintainer="Junpei Kawamoto <junpei@storewise.tech>"
LABEL description="A docker image that provides jq with curl"

USER root
RUN apk add --no-cache jq=1.6-r1

USER curl_user
ENTRYPOINT ["/bin/sh"]
