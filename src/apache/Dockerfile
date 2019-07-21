# Creating apache environment

FROM ubuntu

MAINTAINER BugsBunnies1

RUN apt-get update && apt-get install -y apache2 && apt-get clean && rm -rf /var/lib/apt/lists/*

CMD ["mkdir /var/run/apache2"]
CMD ["source /etc/apache/envvars"]

ENV APACHE_RUN_DIR /etc/apache2/envvars
ENV APACHE_RUN_USER www-data
ENV APACHE_RUN_GROUP www-data
ENV APACHE_LOG_DIR /var/log/apache2

EXPOSE 82

CMD ["/usr/sbin/apache2", "-D", "FOREGROUND"]
