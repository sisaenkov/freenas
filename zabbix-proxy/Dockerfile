FROM zabbix/zabbix-proxy-sqlite3:alpine-3.4.15

ARG BUILD_DATE
ARG VERSION=3.4.15

LABEL org.label-schema.build-date=$BUILD_DATE \
      org.label-schema.vcs-url="https://github.com/sisaenkov/freenas10/tree/master/zabbix-proxy" \
      org.label-schema.version=$VERSION \
      org.label-schema.schema-version="1.0"

LABEL org.freenas.interactive="false"				\
      org.freenas.version=$VERSION				\
      org.freenas.upgradeable="false"				\
      org.freenas.expose-ports-at-host="false"			\
      org.freenas.autostart="true"				\
      org.freenas.settings="[					\
          {							\
              \"env\": \"ZBX_PROXYMODE\",			\
              \"descr\": \"0\",					\
              \"optional\": false				\
          },							\
          {							\
              \"env\": \"ZBX_HOSTNAME\",			\
              \"descr\": \"Proxy hostname\",			\
              \"optional\": false				\
          },							\
          {							\
              \"env\": \"ZBX_SERVER_HOST\",			\
              \"descr\": \"Server IP/hostname\",		\
              \"optional\": false				\
          },							\
          {							\
              \"env\": \"ZBX_SERVER_PORT\",			\
              \"descr\": \"Server port (e.g. 10051)\",		\
              \"optional\": false				\
          }							\
      ]"
