FROM centos

ADD td.repo /etc/yum.repos.d/td.repo
RUN yum update -y
RUN yum install -y td-agent

RUN curl -OL /usr/bin/jq http://stedolan.github.io/jq/download/linux64/jq > /usr/local/bin/jq
RUN chmod +x /usr/local/bin/jq

RUN echo "PATH=/usr/lib64/fluent/ruby/bin:\$PATH" >> /root/.bashrc
 
EXPOSE 24224
 
MAINTAINER tmtk75 "https://github.com/tmtk75"

