FROM ubuntu:trusty
MAINTAINER Glen Stummer <vglen@mpls.io>

ENV JAVA_VER jdk-7u80
ENV JAVA_LINK jdk1.7
ENV JAVA_DIR jdk1.7.0_80

ADD files/${JAVA_VER}-linux-x64.tar.gz /opt/

RUN ln -s /opt/${JAVA_DIR} /opt/${JAVA_LINK}

COPY files/*.jar /opt/${JAVA_LINK}/jre/lib/security/

ENV JAVA_HOME /opt/${JAVA_LINK}
