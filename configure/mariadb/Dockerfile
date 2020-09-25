FROM mariadb:latest
ARG MYSQL_UID
ARG MYSQL_GID
ENV MYSQL_UID ${MYSQL_UID}
ENV MYSQL_GID ${MYSQL_GID}

RUN usermod -u $MYSQL_UID mysql \
&& groupmod -g $MYSQL_GID mysql \
&& chown -R mysql:mysql /var/lib/mysql \
&& chown -R mysql:mysql /var/run/mysqld
