# Output Socket

Reads text based messages from Kafka topic and outputs to socket

## Features

- Reads text based messages from Kafka
- Outputs text based messages to socket
  - Remote connection as a client or local listening socket
  - UDP or TCP  (udp is not supported when client mode used)

## Release Notes

Upgraded output-socket to 3.1.0:

- kafka group id now set using APPLICATION_ID environment variable
- upgrade all dependencies
- log4j.properties now loaded from filesystem
- fixed sonarqube reliability rating failure(s)

 
 