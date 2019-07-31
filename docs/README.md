## Introduction

The Open IoT Edge project brings industry leading software into an
[edge server](https://en.wikipedia.org/wiki/Edge_computing "wikipedia.org")
<sup title="wikipedia.org"><i class="fas fa-external-link-alt fa-xs"></i></sup>
for integrating and automating business processes with on-site IoT devices.

The server can be deployed on-site or in the cloud - close to your integrations.

It uses <img src="https://www.docker.com/sites/default/files/d8/Docker-R-Logo-08-2018-Monochomatic-RGB_Moby-x1.png" alt="Docker" width="16"/>
[Docker](https://www.docker.com) to compose the following components into a full featured, easy to use edge server:

- <img src="https://grafana.com/img/fav32.png" alt="Grafana" width="16"/> [Grafana](https://grafana.com/) - Beautiful analytics, monitoring, and user interface
- <img src="https://nodered.org/favicon.ico" alt="Node-Red" width="16"/> [Node-Red](https://nodered.org) - Flow-based automation for the Internet of Things
- <img src="https://iot-edge.github.io/iot-edge-docs/_media/iot-edge-green-bg-16.png" width="16"/> [IoT-Edge](https://github.com/iot-edge) - Device management and automation plugins
- <img src="https://graphiteapp.org/img/favicon-32x32.png" alt="Graphite" width="16"/> [Graphite](https://graphiteapp.org/) - Time-Series database for metrics storage
- <img src="https://avatars0.githubusercontent.com/u/8270030?s=200&v=4" alt="Statsd" width="16"/> [Statsd](https://www.npmjs.com/package/statsd) - Realtime metrics collection and aggregation
- <img src="https://github.com/grafana/loki/raw/master/docs/logo.png" alt="Loki" width="16"/> [Loki](https://grafana.com/loki) - Activity database for event and log storage
- <img src="https://mosquitto.org/favicon-16x16.png" alt="Mosquitto" width="16"/> [Mosquitto](https://mosquitto.org) - IoT sensor data bus
- <img src="https://docsify.js.org/_media/favicon.ico" alt="Docsify" width="16"/> [Docsify](https://docsify.js.org) - A magical documentation site generator
- <img src="https://www.nginx.com/wp-content/uploads/2019/01/nginx-favicon.png" alt="Nginx" width="16"/> [Nginx](https://www.nginx.com) - Enterprise grade routing, logging, and security

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

Copyright (c) 2019 [Microclimates](https://github.com/microclimates) and [Open IoT Edge contributors](https://github.com/iot-edge/iot-edge/graphs/contributors)