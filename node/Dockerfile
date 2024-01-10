FROM qboson-docker-registry-vpc.cn-beijing.cr.aliyuncs.com/qboson/centos7.9:latest
MAINTAINER "liuc"
#RUN wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
COPY install.sh /root/.nvm/
RUN bash /root/.nvm/install.sh
RUN source ~/.nvm/nvm.sh && \
nvm install v16.19.1 && \
nvm alias default 16.19.1 && \
npm install -g pnpm && \
npm install -g pm2 && \
npm install -g yarn
