# kafka version = 2.8.1 [latest]
# https://www.confluent.io/hub/confluentinc/kafka-connect-jdbc
# get image from strimzi repository
# https://quay.io/repository/strimzi/kafka
FROM quay.io/strimzi/kafka:latest-kafka-2.8.1
# using root user
USER root:root
# create dirs
RUN mkdir -p /opt/kafka/plugins/kafka-connect-jdbc

# copy jar files
COPY ./jars/kafka-connect-jdbc/ /opt/kafka/plugins/kafka-connect-jdbc/
# user
USER 1001