FROM ubuntu:14.04
MAINTAINER Vince lee.wenzhu@gmail.com
RUN apt-get update && apt-get install -y wget
RUN wget http://nodejs.org/dist/v0.12.4/node-v0.12.4-linux-x64.tar.gz
RUN tar -zxvf node-v0.12.4-linux-x64.tar.gz \
    && cd node-v0.12.4-linux-x64 \
    && mv bin/* /usr/local/bin/ \
    && mv lib/node_modules /usr/local/lib/ \
    && cd ~ \
    && rm -rf *
WORKDIR /root
CMD ["/bin/bash"]


#ADD echo.sh /root/echo.sh
#CMD ["sh", "echo.sh"]