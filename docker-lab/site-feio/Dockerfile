FROM centos/systemd
RUN yum -y install httpd; yum clean all; systemctl enable httpd.service
EXPOSE 80
CMD ["httpd", "-D", "FOREGROUND"]
COPY ./docker.png /var/www/html/.
COPY ./home.html /var/www/html/.