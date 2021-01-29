# Observability Stack

An example docker compose template for common observability tools

Includes the following images

* Graphite with StatsD
* Grafana
* Prometheus
* PushGateway (Prometheus scrapper gateway)
* Elasticsearch
* Logstash
* Kibana


## Running

```$ docker-compose up```

The docker-compose file sets up a dedicated network for all these tools to be able to talk to each other.
The containers bind-mount to the relevant folders under `./data` in order to persist the data.
