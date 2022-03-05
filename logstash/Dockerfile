# Main spring-boot server runner
FROM docker.elastic.co/logstash/logstash-oss:8.0.1-amd64
VOLUME /data/conf/
VOLUME /data/logs/
#CMD sleep 10000000
CMD tail -f -n +1 /data/logs/out.log | /usr/share/logstash/bin/logstash -f /data/conf/log.conf

