# Output Socket

Reads text based messages from Kafka topic and outputs to socket

## Features

- Reads text based messages from Kafka
- Outputs text based messages to socket
  - Remote connection as a client or local listening socket
  - UDP or TCP  (udp is not supported when client mode used)

## Release Notes

- removed stale camel settings from resources
- removed MONITORING_PROMETHEUS_PORT from env settings (wasn't used)
- added prometheus settings to JAVA_OPTS
- added units to README.md for OUTPUT_SOCKET_DELAY
- now manually commits kafka offset when socket transmit completes
- upgraded apache-camel-microservice to add inactivity healthcheck
- client connection now uses object based encoding instead of textline; allows multi-line message to be handled by one transmit

 
 