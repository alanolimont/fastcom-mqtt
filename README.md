# Docker Container with Fast.com CLI sending data directly to MQTT Broker 

This is the repository for the blog post:
https://www.simonjenny.dev/docker-container-mit-fast-com-cli-welches-die-resultate-an-einen-mqtt-broker-sendet/ (German)

The Docker needs the following ENV Variables:

SLEEP : Seconds between measures

MQTT_SERVER : IP/Address of MQTT Server

MQTT_DOWN : Topic for Download Value

MQTT_UP : Topic for Upload Value


Optional:

MQTT_USER: MQTT Username

MQTT_PASS: MQTT Password



Example:

```
docker run -e SLEEP='3600' -e MQTT_DOWN='edge/down' -e MQTT_UP='edge/up' -e MQTT_SERVER_='10.10.10.10' simonjenny/fastcom-mqtt:latest
```
