FROM jboss/wildfly:9.0.2.Final

### configuracao do standalone.xml customizado
RUN rm -f /opt/jboss/wildfly/standalone/configuration/standalone.xml
COPY standalone.xml /opt/jboss/wildfly/standalone/configuration/standalone.xml

EXPOSE 8080
EXPOSE 8787

ENTRYPOINT /opt/jboss/wildfly/bin/standalone.sh -b 0.0.0.0 -bmanagement 0.0.0.0 --debug
