FROM java:8

# install drill
ADD ./manage.sh /opt/manage.sh
RUN /opt/manage.sh bootstrap

# expose web server and api port
EXPOSE 8047 31010

# start a server and an repl
# TODO start drillbit and ipython
CMD ["/opt/apache-drill-1.7.0/bin/drill-embedded"]
