# sisaenkov/freenas10-unifi

[![](https://images.microbadger.com/badges/version/sisaenkov/freenas10-unifi:5.9.29.svg)](https://microbadger.com/images/sisaenkov/freenas10-unifi:5.9.29) [![](https://images.microbadger.com/badges/image/sisaenkov/freenas10-unifi.svg)](https://microbadger.com/images/sisaenkov/freenas10-unifi) ![](https://img.shields.io/docker/pulls/sisaenkov/freenas10-unifi.svg) ![](https://img.shields.io/docker/stars/sisaenkov/freenas10-unifi.svg) [![](https://img.shields.io/badge/github-repo-brightgreen.svg)](https://github.com/sisaenkov/freenas10/tree/master/unifi)

Ubiquiti Networks UniFi Controller with FreeNAS metadata.

![](http://cluster015.ovh.net/~pfsikbev/images/partenaires/ubiquiti-unifi-logo.png)

## Overview
* Based on [goofball222/unifi](https://hub.docker.com/r/goofball222/unifi).
* Optimized for FreeNAS Corral docker machine by adding special labels in Dockerfile.

This container follows the latest UniFi current stable/general availability release.

## Usage

The container only has a single environment variable to pass to the container
* `TZ` - Configures the timezone, e.g. "Europe/Moscow"
- If you don't know your timezone value, you can look it up (see: https://en.wikipedia.org/wiki/List_of_tz_database_time_zones)

This container exposes two volumes:
* `/usr/lib/unifi/data` - UniFi configuration data and DBs
* `/usr/lib/unifi/cert` - UniFi certificates

This container exposes the following ports (see: https://help.ubnt.com/hc/en-us/articles/218506997-UniFi-Ports-Used):
* `3478/udp` (port used for STUN connection)
* `6789/tcp` (port used for throughput measurement from Android/iOS app)
* `8080/tcp` (port for UAP/USW/USG to inform controller)
* `8443/tcp` (port for controller GUI / API)
* `8880/tcp` (port for HTTP portal redirect)
* `8843/tcp` (port for HTTPS portal redirect)
* `10001/udp` (port used for UBNT discovery broadcasts - L2/same subnet **only**)

## Upgrading

**It is highly recommended to backup your data prior to installing updates.**

**This can be done by exporting a .unf file from the UniFi interface to be reimported if required. Database rollback from newer to older versions isn't always possible.**
