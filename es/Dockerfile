FROM docker.elastic.co/elasticsearch/elasticsearch:6.3.0
COPY --chown=elasticsearch:elasticsearch elasticsearch.yml /usr/share/elasticsearch/config/
ADD ik/elasticsearch-analysis-ik-6.3.0.zip /tmp/
RUN unzip /tmp/elasticsearch-analysis-ik-6.3.0.zip -d /usr/share/elasticsearch/plugins/ik

