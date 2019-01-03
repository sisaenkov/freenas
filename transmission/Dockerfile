FROM sisaenkov/transmission:latest

ARG BUILD_DATE
ARG VERSION=2.94

LABEL org.label-schema.build-date=$BUILD_DATE \
      org.label-schema.vcs-url="https://github.com/sisaenkov/freenas10/tree/master/transmission" \
      org.label-schema.version=$VERSION \
      org.label-schema.schema-version="1.0"

LABEL org.freenas.interactive="false"				\
      org.freenas.version=$VERSION				\
      org.freenas.upgradeable="true"				\
      org.freenas.expose-ports-at-host="true"			\
      org.freenas.autostart="true"				\
      org.freenas.web-ui-protocol="http"			\
      org.freenas.web-ui-port="9091"				\
      org.freenas.web-ui-path=""				\
      org.freenas.port-mappings="9091:9091/tcp,10894:10894/tcp,10894:10894/udp" \
      org.freenas.volumes="[					\
          {							\
              \"name\": \"/config\",				\
              \"descr\": \"Config storage space\"		\
          },							\
          {							\
              \"name\": \"/downloads\",				\
              \"descr\": \"Downloads volume\"			\
          }							\
      ]"							\
      org.freenas.settings="[					\
          {							\
              \"env\": \"TZ\",					\
              \"descr\": \"Timezone - eg Europe/Moscow\",	\
              \"optional\": true				\
          },							\
          {							\
              \"env\": \"PGID\",				\
              \"descr\": \"GroupID\",				\
              \"optional\": true				\
          },							\
          {							\
              \"env\": \"PUID\",				\
              \"descr\": \"UserID\",				\
              \"optional\": true				\
         }							\
      ]"
