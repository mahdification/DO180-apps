FROM registry.access.redhat.com/ubi7/ubi:7.7
MAINTAINER Mahdi Hashemi <mahdification@gmail.com>
LABEL description="A custom Apache contianer based on UBI 7"
RUN yum install -y httpd && \
	yum clean all
RUN echo "Hello from Dockerfile" > /var/www/html/index.html
EXPOSE 80
CMD ["httpd", "-D", "FOREGROUND"]