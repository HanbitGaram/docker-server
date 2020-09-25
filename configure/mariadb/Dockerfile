FROM mariadb:latest

ARG MYSQL_UID
ARG MYSQL_GID

RUN usermod -u $MYSQL_UID mysql; groupmod -g $MYSQL_GID mysql;

RUN chown -R mysql:mysql /var/lib/mysql /var/run/mysqld