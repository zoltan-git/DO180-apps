FROM ubi8/ubi:8.3

MAINTAINER Zoltan zoltan@email.com

ENV zoltan=ex180pass

LABEL do180="This is great"

RUN 	yum install -y httpd && \
	yum clean all

EXPOSE 80

ADD ./src/ /var/www/html/

COPY index.html /var/www/html/

CMD ["/usr/bin/httpd", "-D", "FOREGROUND"]

