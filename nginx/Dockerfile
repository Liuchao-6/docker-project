FROM qboson-docker-registry-vpc.cn-beijing.cr.aliyuncs.com/qboson/centos7.9:latest

RUN yum install -y epel-release && \
yum install -y nginx

ADD nginx.conf /etc/nginx

EXPOSE 80

CMD ["nginx","-g","daemon off;"]
