![logo](https://assets.zabbix.com/img/logo/zabbix_logo_500x131.png)

### Description

Zabbix Agent 3.4.15

## Environment Variables

### `ZBX_HOSTNAME`

This variable is unique, case sensitive hostname. By default, value is `hostname` of the container. It is ``Hostname`` parameter in ``zabbix_agentd.conf``.

### `ZBX_SERVER_HOST`

This variable is IP or DNS name of Zabbix server or Zabbix proxy. By default, value is `zabbix-server`. It is ``Server`` parameter in ``zabbix_agentd.conf``. It is allowed to specify Zabbix server or Zabbix proxy port number using ``ZBX_SERVER_PORT`` variable. It make sense in case of non-default port for active checks.

### `ZBX_ACTIVESERVERS`

The variable is comma separated list of allowed Zabbix server or proxy hosts for connections to Zabbix agent container. You may specify port of Zabbix server or Zabbix proxy in such syntax: ``zabbix-server:10061,zabbix-proxy:10072``.

Additionally the image allows to specify many other environment variables listed below:

```
ZBX_SOURCEIP=
ZBX_ENABLEREMOTECOMMANDS=0
ZBX_LOGREMOTECOMMANDS=0
ZBX_STARTAGENTS=3
ZBX_HOSTNAMEITEM=system.hostname
ZBX_METADATA=
ZBX_METADATAITEM=
ZBX_REFRESHACTIVECHECKS=120
ZBX_BUFFERSEND=5
ZBX_BUFFERSIZE=100
ZBX_MAXLINESPERSECOND=20
ZBX_LISTENIP=
ZBX_UNSAFEUSERPARAMETERS=0
ZBX_TLSCONNECT=unencrypted
ZBX_TLSACCEPT=unencrypted
ZBX_TLSCAFILE=
ZBX_TLSCRLFILE=
ZBX_TLSSERVERCERTISSUER=
ZBX_TLSSERVERCERTSUBJECT=
ZBX_TLSCERTFILE=
ZBX_TLSKEYFILE=
ZBX_TLSPSKIDENTITY=
ZBX_TLSPSKFILE=
```
