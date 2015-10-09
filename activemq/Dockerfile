FROM dmitrybespalov/centos-7.1.1503-java7.jre

MAINTAINER Dmitry Bespalov <bespalovdn@gmail.com>

RUN mkdir -p /opt/activemq

WORKDIR /opt/activemq

COPY source /opt/activemq

EXPOSE 8161
EXPOSE 61616

CMD ["/opt/activemq/bin/activemq", "console"]
