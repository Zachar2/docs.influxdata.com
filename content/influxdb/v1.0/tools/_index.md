---
title: Tools
aliases:
    - influxdb/v1.0/clients/
    - influxdb/v1.0/write_protocols/json/
---

This section covers the available tools for interacting with InfluxDB.

## [CLI/Shell](/influxdb/v1.0/tools/shell/)

InfluxDB's Command Line Interface (`influx`) is an interactive shell for the
HTTP API that comes with every InfluxDB package.
Use `influx` to write data (manually or from a file), query data interactively,
and view query output in different formats:

![CLI GIF](/img/influxdb/cli-1.0-beta.gif)

Go straight to the documentation on:

* [Launching `influx`](/influxdb/v1.0/tools/shell/#launch-influx)
* [Writing data with `influx`](/influxdb/v1.0/tools/shell/#write-data-to-influxdb-with-insert)

## [API Reference](/influxdb/v1.0/tools/api/)

Reference documentation for InfluxDB's HTTP API.

Go straight to the reference documentation on:

* [Writing data with the HTTP API](/influxdb/v1.0/tools/api/#write)
* [Querying data with the HTTP API](/influxdb/v1.0/tools/api/#query)

For friendlier documentation, see the guides on
[writing data](/influxdb/v1.0/guides/writing_data/) and
[querying data](/influxdb/v1.0/guides/querying_data/) with the HTTP API.

## [API Client Libraries](/influxdb/v1.0/tools/api_client_libraries/)

The list of client libraries for interacting with InfluxDB.

## [Web Admin Interface](/influxdb/v1.0/tools/web_admin/)

InfluxDB's built-in web administration GUI.
We recommend using the HTTP API or the CLI instead of the Web Admin.

## [Influx Inspect](/influxdb/v1.0/tools/influx_inspect/)

Influx Inspect is a tool designed to view detailed information about on disk shards, as well as export data from a shard to line protocol that can be inserted back into the database.

## [Grafana Graphs and Dashboards](http://docs.grafana.org/datasources/influxdb/)

Grafana is a convenient dashboard tool for visualizing time series data.
It was originally built for Graphite, modeled after Kibana, and since been updated to support InfluxDB.

{{% warn %}} Because of the [changes](/influxdb/v0.11/concepts/010_vs_011/#breaking-api-changes) to the `SHOW SERIES` and `SHOW TAG VALUES` formats in InfluxDB 0.11, InfluxDB 1.0 will not work with the Query Editor in Grafana 2.6.
This issue does not affect existing queries and dashboards or users working with Grafana 3.0. {{% /warn %}}

## Service Plugins

InfluxDB accepts writes over
[UDP](/influxdb/v1.0/tools/udp/)
and provides an easy way to set up
[Graphite](/influxdb/v1.0/tools/graphite/),
[CollectD](/influxdb/v1.0/tools/collectd/),
and [OpenTSDB](/influxdb/v1.0/tools/opentsdb/) as input sources.
