# Installing Java7 JRE on top of CentOS 7

FROM centos:7.1.1503

RUN yum install -y tar wget

WORKDIR /opt

# 1. get tar
# 2. extract tar
# 3. update alternatives
RUN wget --no-cookies --no-check-certificate --header "Cookie: gpw_e24=http%3A%2F%2Fwww.oracle.com%2F; oraclelicense=accept-securebackup-cookie" "http://download.oracle.com/otn-pub/java/jdk/7u71-b14/jre-7u71-linux-x64.tar.gz" \
  && tar xvf jre-7u71-linux-x64.tar.gz \
  && chown -R root: jre1.7.0_71 \
  && ln -s jre1.7.0_71 jre \
  && alternatives --install /usr/bin/java java /opt/jre/bin/java 1

