FROM sisaenkov/ivideon-server:latest

ARG BUILD_DATE
ARG VERSION=3.7.0.2642

LABEL org.label-schema.build-date=$BUILD_DATE \
      org.label-schema.vcs-url="https://github.com/sisaenkov/freenas10/tree/master/ivideon-server" \
      org.label-schema.version=$VERSION \
      org.label-schema.schema-version="1.0"

LABEL org.freenas.interactive="false" \
      org.freenas.version=$VERSION \
      org.freenas.upgradeable="false" \
      org.freenas.expose-ports-at-host="false"\
      org.freenas.autostart="true" \
      org.freenas.port-mappings="8080:8080/tcp" \
      org.freenas.volumes="[                                            \
          {                                                             \
              \"name\": \"/config\",                                    \
              \"descr\": \"Config storage space\"                       \
          },                                                            \
          {                                                             \
              \"name\": \"/archive\",                                   \
              \"descr\": \"video archive directory [optional]\"         \
          }                                                             \
      ]"                                                                \
      org.freenas.settings="[                                           \
          {                                                             \
              \"env\": \"EMAIL\",                                       \
              \"descr\": \"Your ivideon.com account\"                   \
          },                                                            \
          {                                                             \
              \"env\": \"SERVER_NAME\",                                 \
              \"descr\": \"Ivideon server name without spaces (displayed in Ivideon Client and Web UI)\"    \
          }                                                             \
      ]"
