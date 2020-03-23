# Encode ACP128 / OS-OTG 

Encodes GCI+ Avro `MaritimeContact` messages into ACP-128 wrapped OS-OTG XCTC messages.

## Features

- Encodes OS-OTG XCTC messages from GCI+ `MaritimeContacts` messages 
- Encodes ACP-128 messages from OS-OTG XCTC messages

## Release Notes

- Enhanced http healthcheck(s) to report error state when service(s) encounter idle/dead state (occurs when topic(s) referred 
to by KAFKA_INPUT_TOPICS have not been created prior to starting the service)

 
 