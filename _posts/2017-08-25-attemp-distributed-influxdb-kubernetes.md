---
title: An attempt to make InfluxDB scable on a Azure cluster powered by Kubernetes
date: 2017-08-25 19:45:50
---

[InfluxDB] is a fast, horizontally scable time-series database that is well-known used in real time analytics and IOT applications.
The enterprise version shows an impressive writing performance in [this experiment] where it can write up to 11 milions values per second
with 32 data nodes. It also offers a rich SQL-like query language and a HTTP API which is easy for integration. So we have a plan to make some benchmarks
with InfluxDB to see if choosing InfluxDB is a good move compared to our current database. This blog demonstrates our attempts to install and make InfluxDB scable (without using enterprise version)
on a Azure cluster powered by Kubernetes.

## Install InfluxDB on a Azure cluster with Kubernetes

Why Azure and Kubernetes? At eSmart Systems we use Azure in most of our infrastructure components. [Kubernetes] is a matured platform designed for automating deploying, scaling, operating
application containers and is currently used to deploy our time-series services. Deploying InfluxDB on the same cluster will reduce overhead comuting data across service and database.




## Attempt to make it scable
## Use acs-engine to create a more flexible Kubernetes cluster