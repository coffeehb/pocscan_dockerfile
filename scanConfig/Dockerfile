#++++++++++++++++++++++++++++++++++++++
# Debian 8 PHP-Nginx Docker container
#++++++++++++++++++++++++++++++++++++++

FROM bishe/env:1.0 
MAINTAINER kbz 

COPY superenv.conf /etc/supervisor/conf.d/superenv.conf

COPY supervisord.conf /etc/supervisor/supervisord.conf

COPY init.sh /tmp/init.sh
RUN chmod 777 /tmp/init.sh

ENTRYPOINT ["/etc/init.d/supervisor","start"]
