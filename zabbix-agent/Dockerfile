FROM zabbix/zabbix-agent:alpine-3.4.15
LABEL org.freenas.interactive="false"			\
      org.freenas.version="3.4.15"			\
      org.freenas.upgradeable="true"			\
      org.freenas.expose-ports-at-host="true"		\
      org.freenas.autostart="true"			\
      org.freenas.port-mappings="10050:10050/tcp"	\
      org.freenas.settings="[				\
          {						\
              \"env\": \"ZBX_HOSTNAME\",		\
              \"descr\": \"hostname\",			\
              \"optional\": false			\
          },						\
          {						\
              \"env\": \"ZBX_SERVER_HOST\",		\
              \"descr\": \"Server IP/hostname\",	\
              \"optional\": false			\
          },						\
          {						\
              \"env\": \"ZBX_ACTIVESERVERS\",		\
              \"descr\": \"Active server IP[:PORT]\",	\
              \"optional\": true			\
          },						\
          {						\
              \"env\": \"ZBX_SERVER_PORT\",		\
              \"descr\": \"Server port (e.g. 10051)\",	\
              \"optional\": true			\
          },						\
          {						\
              \"env\": \"ZBX_ENABLEREMOTECOMMANDS\",	\
              \"descr\": \"0 - false, 1 - true\",	\
              \"optional\": true			\
          },						\
          {						\
              \"env\": \"ZBX_LOGREMOTECOMMANDS\",	\
              \"descr\": \"0 - false, 1 - true\",	\
              \"optional\": true			\
          }						\
      ]"
