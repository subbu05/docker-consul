FROM centos:7

MAINTAINER Subbu M

WORKDIR /root

RUN yum clean all && \
    yum install -y unzip dnsmasq && \
    yum update -y && \
    curl -o consul.zip https://releases.hashicorp.com/consul/0.7.0/consul_0.7.0_linux_amd64.zip && \
    unzip consul.zip && \
    chmod 755 consul && \
    cp consul /usr/local/bin && \
    rm -rf ./*
