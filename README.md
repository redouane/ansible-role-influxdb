Ansible Role: InfluxDB
======================

Installs and configures influxdb

Requirements
------------

None

Role Variables
--------------

```yaml

influxdb_version: 0.9.4.2

#dirs
influxdb_meta_dir: /var/opt/influxdb/meta
influxdb_data_dir: /var/opt/influxdb/data
influxdb_wal_dir: /var/opt/influxdb/wal
influxdb_hh_dir: /var/opt/influxdb/hh

#meta
influxdb_reporting_disabled: false
influxdb_hostname: localhost
influxdb_bind_address: :8088

#retention
influxdb_retention_enabled: true

#admin
influxdb_admin_enabled: true
influxdb_admin_bind_address: :8083

```

License
-------

BSD