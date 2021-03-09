FROM k8s.gcr.io/kubernetes-zookeeper:1.0-3.4.10


ENV ZK_USER=zookeeper

#Copy zookeeper-ready script to bin
COPY zookeeper-ready /opt/zookeeper/bin
COPY zookeeper-startup /opt/zookeeper/bin

RUN chown -R "$ZK_USER:$ZK_USER" /opt/zookeeper/bin/zookeeper-ready
RUN chown -R "$ZK_USER:$ZK_USER" /opt/zookeeper/bin/zookeeper-startup

RUN chmod 700 /opt/zookeeper/bin/zookeeper-ready
RUN chmod 700 /opt/zookeeper/bin/zookeeper-startup
