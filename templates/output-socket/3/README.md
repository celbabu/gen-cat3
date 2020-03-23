# Output Socket

Reads text based messages from Kafka topic and outputs to socket

## Features

- Reads text based messages from Kafka
- Outputs text based messages to socket
  - Remote connection as a client or local listening socket
  - UDP or TCP  (udp is not supported when client mode used)

## Release Notes

Upgraded output-socket to 3.1.0:

- JAVA_OPTS was referring to the wrong version (e.g. previous release) for prometheus agent

 
 