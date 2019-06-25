# <img src="https://github.com/iot-edge/iot-edge-docs/raw/master/docs/_media/iot-edge-green-bg-100.png" width="60"/><br/>Open IoT Edge Documentation

This repo contains documentation pages for the [IoT Edge Server](https://github.com/iot-edge/iot-edge/) project.

The /docs directory contains raw [markdown](https://www.markdownguide.org) files and image assets.

These files are rendered on the browser using the [Docsify](https://docsify.js.org) documentation runner.

## [Documentation Site](https://iot-edge.github.io/iot-edge-docs/#/)

## Editing Documentation

The doc pages can be edited by issuing a pull request to this repository.

To setup a local doc server, install docsify:
```bash
npm install -g docsify
```

Then clone the repository:
```
git clone https://github.com/iot-edge/iot-edge-docs.git
```

Then run the docsify server in the directory:
```
cd iot-edge-docs
docsify serve docs
```