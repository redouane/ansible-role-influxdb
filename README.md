Ansible Role: InfluxDB
======================

[![Build Status](https://travis-ci.org/redouane/ansible-role-influxdb.svg?branch=master)](https://travis-ci.org/redouane/ansible-role-influxdb)

Installs and configures influxdb

Requirements
------------

None

Role Variables
--------------

```yaml

influxdb_version: 0.9.5
influxdb_download_url: https://s3.amazonaws.com/influxdb

#dirs
influxdb_meta_dir: /var/lib/influxdb/meta
influxdb_data_dir: /var/lib/influxdb/data
influxdb_wal_dir: /var/lib/influxdb/wal
influxdb_hh_dir: /var/lib/influxdb/hh

#meta
influxdb_reporting_disabled: false
influxdb_hostname: localhost
influxdb_bind_address: :8088

#retention
influxdb_retention_enabled: true

#admin
influxdb_admin_enabled: true
influxdb_admin_bind_address: :8083

#graphite
influxdb_graphite_config:

```


Todo
----
- fix role idempotency / influxdb reconfiguration  after /tmp/influxdb.conf gets erased (after machine restarts mostly)

License
-------

BSD