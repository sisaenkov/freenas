FROM zabbix/zabbix-proxy-sqlite3:alpine-3.4.15
LABEL org.freenas.interactive="false"				\
      org.freenas.version="3.4.15"				\
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
