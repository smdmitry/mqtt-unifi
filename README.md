# mqtt-unifi
MQTT integration for Ubiquiti UniFi controller

## Docker Compose

```yml
version: '3'

services:

  unifi:
    build: https://github.com/smdmitry/mqtt-unifi.git

    restart: always

    environment:
      - MQTT_ID=unifi
      - MQTT_PATH=unifi
      - MQTT_HOST=mqtt://<ip address of mqtt broker>
      - MQTT_USERNAME=<mqtt username>
      - MQTT_PASSWORD=<mqtt password>
      - UNIFI_HOST=<ip address of unifi controller>
      - UNIFI_USERNAME=<unifi username>
      - UNIFI_PASSWORD=<unifi password>
```
