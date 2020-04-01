FROM ubi7/ubi:7.7

MAINTAINER Dhruv Dave dave_dhruv@yahoo.com

LABEL description="dave_dhruv DO180: A custom Apache container based on UBI 7."

RUN yum install -y httpd && \
    yum clean all

RUN echo "dave_dhruv DO180: Hello from Dockerfile" > /usr/share/httpd/noindex/index.html

EXPOSE 80

ENTRYPOINT ["httpd", "-D", "FOREGROUND"]

