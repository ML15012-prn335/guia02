FROM postgres:9.6.3-alpine
MAINTAINER rene eduardo mendoza lemus
COPY post_v2.sql /docker-entrypoint-initdb.d/ 
ENV PGDATA /var/lib/postgresql/data 
VOLUME /var/lib/postgresql/data 
COPY docker-entrypoint.sh / 
ENTRYPOINT ["/docker-entrypoint.sh"]
EXPOSE 5432 
CMD ["postgres"]
