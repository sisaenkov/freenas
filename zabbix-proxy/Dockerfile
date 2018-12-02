FROM zabbix/zabbix-proxy-sqlite3:alpine-3.4.14
LABEL org.freenas.interactive="false"				\
      org.freenas.version="3.4.14"				\
      org.freenas.upgradeable="false"				\
      org.freenas.expose-ports-at-host="false"			\
      org.freenas.autostart="true"				\
      org.freenas.volumes="[					\
          {							\
              \"name\": \"/var/lib/zabbix\",			\
              \"descr\": \"Database directory\"			\
          }							\
      ]"							\
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
              \"descr\": \"Zabbix server IP/hostname\",		\
              \"optional\": false				\
          },							\
          {							\
              \"env\": \"ZBX_SERVER_PORT\",			\
              \"descr\": \"Zabbix server port (e.g. 10051)\",	\
              \"optional\": false				\
          },							\
          {							\
              \"env\": \"TERM\",				\
              \"descr\": \"xterm\",				\
              \"optional\": true				\
          }							\
      ]"
