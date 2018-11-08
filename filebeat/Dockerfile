FROM docker.elastic.co/beats/filebeat:6.4.3

COPY tracking.log /var/log/tracking.log
COPY filebeat.yml /usr/share/filebeat/filebeat.yml

USER root

RUN chown root:filebeat /var/log/tracking.log
RUN chown root:filebeat /usr/share/filebeat/filebeat.yml

USER filebeat