FROM   debian:buster
ENV    DEBIAN_FRONTEND noninteractive

# install required packges
RUN apt-get update -qq && \
    apt-get upgrade -y && \
    apt-get install -y php7.3-cli \
    php7.3-mysqlnd php7.3-mysql php7.3-curl php7.3-gd php7.3-soap php7.3-mbstring php7.3-zip php7.3-sqlite php7.3-xml php7.3-dom php7.3-bcmath \
    php-pear curl openssl sudo ca-certificates \
    g++ make cmake libssl-dev libgmp-dev php7.3-dev libpcre3-dev git && \
    apt-get clean autoclean && \
    apt-get autoremove --yes && \
    rm -rf /var/lib/{apt,dpkg,cache,log}/

ADD docker-entrypoint.sh /usr/local/sbin/docker-entrypoint.sh

ENTRYPOINT ["/usr/local/sbin/docker-entrypoint.sh"]

