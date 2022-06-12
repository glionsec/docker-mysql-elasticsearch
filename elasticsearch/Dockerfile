FROM docker.elastic.co/elasticsearch/elasticsearch:7.17.4

COPY ./config/elasticsearch.yml /usr/share/elasticsearch/config/elasticsearch.yml

# Install kuromoji plugin
RUN elasticsearch-plugin  install analysis-kuromoji