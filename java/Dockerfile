FROM qboson-docker-registry-vpc.cn-beijing.cr.aliyuncs.com/qboson/centos7.9:latest
MAINTAINER "liuc"
RUN rm -f /etc/localtime && \
ln -s /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
WORKDIR /usr/local/
ADD jdk-8u391-linux-x64.tar.gz /usr/local/
ADD apache-maven-3.5.2-bin.tar.gz /usr/local/
ENV JAVA_HOME /usr/local/jdk1.8.0_391
ENV JRE_HOME $JAVA_HOME/jre
ENV MAVEN_HOME /usr/local/apache-maven-3.5.2
ENV PATH $JAVA_HOME/bin:$MAVEN_HOME/bin:$PATH
