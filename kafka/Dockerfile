FROM gcr.io/google-samples/k8skafka:v1


ENV KAFKA_USER=kafka

#Copy kafka-ready script to bin
COPY kafka-ready /opt/kafka/bin


RUN chown -R "$KAFKA_USER:$KAFKA_USER" /opt/kafka/bin/kafka-ready
RUN chmod 700 /opt/kafka/bin/kafka-ready
