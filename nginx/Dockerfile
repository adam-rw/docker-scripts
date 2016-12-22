FROM adamwilliams/c7-systemd

ADD src/nginx.repo /etc/yum.repos.d/nginx.repo

RUN ["yum", "install", "-y", "nginx"]

RUN ["systemctl", "enable", "nginx.service"]

EXPOSE 80

CMD ["/usr/sbin/init"]
