---
layout: "influxdb"
page_title: "Provider: InfluxDB"
sidebar_current: "docs-influxdb-index"
description: |-
  The InfluxDB provider configures databases, etc on an InfluxDB server.
---

# InfluxDB V2 Provider

The InfluxDB provider allows Terraform to create Databases in
[InfluxDB](https://influxdb.com/). InfluxDB is a database server optimized
for time-series data.

The provider configuration block accepts the following arguments:

* ``url`` - (Optional) The root URL of a InfluxDB V2 server. May alternatively be
  set via the ``INFLUXDB_URL`` environment variable. Defaults to
  `http://localhost:9999/`.
  
## Example Usage

```hcl
provider "influxdb" {
  url      = "http://influxdb.example.com:9999"
}