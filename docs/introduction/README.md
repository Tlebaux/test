# Introduction

![Docker pulls](https://img.shields.io/docker/pulls/fmartinou/tydom2mqtt)
![License](https://img.shields.io/github/license/fmartinou/tydom2mqtt)
![Travis](https://img.shields.io/travis/fmartinou/tydom2mqtt/master)

**tydom2mqtt** allows you to integrate Deltadore Tydom Hubs to MQTT.

## Quick start

### Run the Docker image
The easiest way to start is to deploy the official _**tydom2mqtt**_ image.

<!-- tabs:start -->
#### **Docker Compose**
```yaml
version: '3'

services:
  tydom2mqtt:
    image: Tlebaux/tydom2mqtt
    container_name: tydom2mqtt
    environment:
      - TYDOM_MAC=001A25XXXXXX
      - TYDOM_PASSWORD=azertypass
      - TYDOM_IP=192.168.1.33
```
#### **Docker**
```bash
docker run -d --name tydom2mqtt \
  -e TYDOM_MAC="001A25XXXXXX" \
  -e TYDOM_PASSWORD="azertypass" \
  -e TYDOM_IP="192.168.1.33" \  
  Tlebaux/tydom2mqtt
```
<!-- tabs:end -->

?> [Please find here all the configuration options.](/configuration/)

!> Are you a Home-Assistant user? \
So maybe take a look at the [Hass.io add-on version](/hass/)!


This project is licensed under the [MIT license](https://github.com/fmartinou/tydom2mqtt/blob/master/LICENSE).

<!-- GitHub Buttons -->
<script async defer src="https://buttons.github.io/buttons.js"></script>
