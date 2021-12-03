FROM mysql:latest
EXPOSE 3306
RUN usermod -u 1000 mysql
ENTRYPOINT ["docker-entrypoint.sh"]
CMD ["mysqld"]