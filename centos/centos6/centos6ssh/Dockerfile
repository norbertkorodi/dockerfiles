FROM centos:6.8
RUN yum -y install openssh openssh-server openssh-clients openssl-libs
RUN cp /etc/ssh/sshd_config /etc/ssh/sshd_config.orig
RUN adduser vagrant
RUN echo vagrant:vagrant | chpasswd

CMD bash /etc/init.d/sshd start && tail -f /dev/null
