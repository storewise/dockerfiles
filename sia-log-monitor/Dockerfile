FROM fluent/fluentd:stable
LABEL maintainer="Junpei Kawamoto <junpei@storewise.tech>"
LABEL description="Monitoring log files of a Sia node and forwarding them to stdout"
LABEL org.opencontainers.image.url="https://github.com/storewise/dockerfiles/tree/master/sia-log-monitor"
LABEL org.opencontainers.image.documentation="https://github.com/storewise/dockerfiles"
LABEL org.opencontainers.image.source="https://github.com/storewise/dockerfiles"
LABEL org.opencontainers.image.vendor="StoreWise"
LABEL org.opencontainers.image.title="Sia log monitor"
LABEL org.opencontainers.image.description="Monitoring log files of a Sia node and forwarding them to stdout"

ENV SIA_DIRECTORY /sia
RUN gem install --no-document fluent-plugin-record-modifier:2.1.0

COPY conf/fluent.conf /fluentd/etc/

USER root
ENTRYPOINT ["/usr/bin/fluentd"]
CMD ["-q", "-c", "/fluentd/etc/fluent.conf", "-p", "/fluentd/plugins"]
