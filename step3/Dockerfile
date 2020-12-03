FROM oracle-12c:created

RUN rm /tmp/create

# (8080) and HTTPS (5500) ports. 
EXPOSE 1521 5500 8080

ADD startdb.sql $ORACLE_HOME/config/scripts/startdb.sql
ADD start /tmp/start
CMD /tmp/start
