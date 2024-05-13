FROM quay.io/prometheus/node-exporter:latest

ENV NODE_ID=none

USER root

COPY conf /etc/node-exporter/
#RUN chmod 777 /etc/node-exporter/docker-entrypoint.sh
RUN chmod +x /etc/node-exporter/docker-entrypoint.sh
#RUN cat /etc/node-exporter/docker-entrypoint.sh

ENTRYPOINT ["/bin/sh", "/etc/node-exporter/docker-entrypoint.sh" ]
#CMD [ "/bin/node_exporter" ]