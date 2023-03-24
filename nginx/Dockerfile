FROM nginx:latest
# COPY default.conf /etc/nginx/conf.d/default.conf
COPY index.html /usr/share/nginx/html/
RUN \
    apt update && mkdir /usr/share/nginx/html/report /usr/share/nginx/html/report && \
    apt install curl openjdk-11-jre/stable-security bash -y && \
    curl -L https://archive.apache.org/dist/jmeter/binaries/apache-jmeter-5.4.1.tgz > /tmp/jmeter.tgz && \
    mkdir -p /opt/ && \
    tar -xvzf /tmp/jmter.tgz -C /opt && \
    rm /tmp/jmeter.tgz
  