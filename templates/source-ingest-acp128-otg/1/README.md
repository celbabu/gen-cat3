# Ingest ACP128 / OS-OTG 

Ingests ACP128 wrapper OS-OTG (XCTC and GOLD) messages and converts to GCI+ `MaritimeContact` messages.

## Features

- Consumes ACP128 messages from a local/remote socket
- Decodes ACP128 messages
- Decodes OS-OTG and generates MaritimeContacts. 

**Be sure to expose the port being used if this stack acts as a receiveing server**

## Release Notes

- Enhanced http healthcheck(s) to report error state when service(s) encounter idle/dead state (occurs when topic(s) referred 
to by KAFKA_INPUT_TOPICS have not been created prior to starting the service)
- Upgraded to avro-lexicon-maritime 3.1.4 (latest as of May 2, 2019)

 
 