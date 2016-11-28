FROM centos:6

MAINTAINER Milan Sulc <sulc@ders.cz>

ENV TERM xterm
ENV USER_UID 1000
ENV USER_NAME ders

RUN yum update && \
    yum upgrade -y && \
    useradd -ms /bin/bash -u $USER_UID $USER_NAME && \
    yum clean all && yum autoremove -y && \
    rm -rf /tmp/* /var/tmp/*

CMD ["/bin/bash"]
