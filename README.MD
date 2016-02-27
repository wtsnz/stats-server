# stats-server

This is a docker-compose configuration that describes the services that I use to collect a bunch of stats.

Essentially, this creates a nearly complete stack of the [Influxdata apps](https://influxdata.com/).

## Services

### InfluxDB

The time-series database.

### Telegraf

The data collector, running in statsd mode.

### Chronograf

The graph part. Considering changing to Grafana as it's slightly better. (Chronograf is incomplete)

## Installation

Make sure you have docker & docker-compose installed on your machine.
Clone the repository and run the stats.py

    git clone https://github.com/wtsnz/stats-server.git
    cd stats-server

## Usage

    docker-compose up -d

## Future

It would be cool to allow enviromental variables to override the defaults in the docker-compose.yml file using [variable substitution](https://github.com/docker/compose/blob/129092b7/docs/yml.md#variable-substitution)
