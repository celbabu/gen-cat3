# Ingest ACP128 / OS-OTG 

Ingests ACP128 wrapper OS-OTG (XCTC and GOLD) messages and converts to GCI+ `MaritimeContact` messages.

## Features

- Consumes ACP128 messages from a local/remote socket
- Decodes ACP128 messages
- Decodes OS-OTG and generates MaritimeContacts. 

**Be sure to expose the port being used if this stack acts as a receiveing server**

## Release Notes

- upgraded ingest-socket to 4.2.1:

    - Fixed byte filtering to handle `\` characters correctly
    - Added content to README.md
    - MESSAGE_START_TOKENS defaults now defined in camel.properties
    - MESSAGE_END_TOKENS defaults now defined in camel.properties

 - removed default env settings in docker-compose.yml that are identical to defaults defined in Dockerfile for
services