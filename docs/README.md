## Introduction

The [Open IoT Edge](https://github.com/iot-edge) project brings industry leading software into an
[edge server](https://en.wikipedia.org/wiki/Edge_computing "wikipedia.org") for integrating and automating business processes with on-site IoT devices.

The server can be deployed on-site or in the cloud - close to your integrations.

It uses 
![docker](https://iot-edge.github.io/iot-edge-docs/_media/icon/docker.png) [Docker](https://www.docker.com) to compose the following components into a full featured edge server:

- ![Grafana](https://iot-edge.github.io/iot-edge-docs/_media/icon/grafana.png) [Grafana](https://grafana.com/) - Beautiful analytics, monitoring, and user interface
- ![nodered](https://iot-edge.github.io/iot-edge-docs/_media/icon/nodered.png) [Node-Red](https://nodered.org) - Flow-based automation for the Internet of Things
- ![iot-edge](https://iot-edge.github.io/iot-edge-docs/_media/icon/iot-edge.png) [IoT-Edge](https://github.com/iot-edge/iot-edge) - Device management and automation plugins
- ![graphite](https://iot-edge.github.io/iot-edge-docs/_media/icon/graphite.png) [Graphite](https://graphiteapp.org/) - Time-Series database for metrics storage
- ![statsd](https://iot-edge.github.io/iot-edge-docs/_media/icon/statsd.png) [Statsd](https://www.npmjs.com/package/statsd) - Realtime metrics collection and aggregation
- ![redis](https://iot-edge.github.io/iot-edge-docs/_media/icon/redis.png) [Redis](https://redis.io) - Performance database, text search, and more
- ![loki](https://iot-edge.github.io/iot-edge-docs/_media/icon/loki.png) [Loki](https://grafana.com/loki) - Activity database for event and log storage
- ![mosquitto](https://iot-edge.github.io/iot-edge-docs/_media/icon/mosquitto.png) [Mosquitto](https://mosquitto.org) - IoT sensor message bus
- ![nginx](https://iot-edge.github.io/iot-edge-docs/_media/icon/nginx.png) [Nginx](https://www.nginx.com) - Enterprise grade routing, logging, and security

## Hardware

The server runs wherever amd64 [<img src="https://www.docker.com/sites/default/files/d8/Docker-R-Logo-08-2018-Monochomatic-RGB_Moby-x1.png" alt="Docker" width="16"/>](https://www.docker.com) Docker runs.

It requires a minimum of 2GB RAM and a hard disk for metrics and logging storage. It runs well on a development laptop or workstation, and should be deployed on a dedicated server with enough RAM, CPU, and hard disk space to
match the installation size.

## Quick Start

Make sure you've installed these prerequisites

- [NodeJS](https://nodejs.org)
- [Docker](https://www.docker.com/products)

Next, build yourself a server in a new folder

```
npm install -g yo generator-edge
yo edge
```

Now start the server

```
npm start
```

And view it from your browser

```
http://localhost:8000/
```

## Project Guidelines

- *Fast* - Quick start, fast iterations
- *Minimal* - Stable core with plugins for customization
- *Open* - Built with open source components, free license
- *Secure* - Enterprise grade security components
- *Supported* - [Developer tools](https://www.npmjs.com/package/generator-edge) and [community support](https://gitter.im/iot-edge/community) forums

## License

May be freely run and distributed under the [MIT license](https://raw.githubusercontent.com/iot-edge/iot-edge/master/LICENSE).

Copyright (c) 2019 [Microclimates](https://github.com/microclimates) and the [Open IoT Edge contributors](https://github.com/iot-edge/iot-edge/graphs/contributors)