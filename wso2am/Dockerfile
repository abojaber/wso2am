From java:8

MAINTAINER ABOJABER@PROGRAMER.COM

COPY ./wso2am-2.1.0.zip ./

RUN apt-get update && \
    apt-get install -y zip && \
    apt-get clean && \
    unzip wso2am-2.1.0.zip -d /tmp && \
    rm wso2am-2.1.0.zip


EXPOSE 9443 9763 8243 8280 10397 7711


WORKDIR /tmp/wso2am-2.1.0

ENTRYPOINT ["bin/wso2server.sh"]