FROM nidarbox/ubuntu:16.04

MAINTAINER Jesus Farfan <jesu.farfan23@gmail.com>

ENV NODE_VERSION 6.11.2
ENV ARCH x64

# Install node and npm
RUN curl -SLO --progress-bar https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.gz \
    && tar xvzf node-v$NODE_VERSION-linux-$ARCH.tar.gz -C /opt \
    && ln -s /opt/node-v$NODE_VERSION-linux-$ARCH/bin/node /usr/local/bin/node \
    && ln -s /opt/node-v$NODE_VERSION-linux-$ARCH/bin/npm /usr/local/bin/npm \
    && rm node-v$NODE_VERSION-linux-$ARCH.tar.gz

# Install latest yarn
RUN curl -o- -L https://yarnpkg.com/install.sh | bash
