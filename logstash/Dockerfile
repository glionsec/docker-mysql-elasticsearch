FROM docker.elastic.co/logstash/logstash:7.17.4

RUN rm -rf /usr/share/logstash/pipeline
COPY pipeline /usr/share/logstash/pipeline
COPY mysql-connector-java-8.0.17.jar /usr/share/logstash/mysql-connector-java-8.0.17.jar

ENV LANG ='en_US.UTF-8' LC_ALL ='en_US.UTF-8'