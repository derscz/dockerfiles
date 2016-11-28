FROM debian:sid

MAINTAINER Milan Sulc <sulc@ders.cz>

ENV DEBIAN_FRONTEND noninteractive

ENV TERM xterm
ENV USER_UID 1000
ENV USER_NAME ders

RUN apt-get update && \
    apt-get upgrade -y && \
    useradd -ms /bin/bash -u $USER_UID $USER_NAME && \
    apt-get clean -y && apt-get autoclean -y && apt-get autoremove -y && \
    rm -rf /var/lib/apt/lists/* /var/lib/log/* /tmp/* /var/tmp/*

CMD ["/bin/bash"]
