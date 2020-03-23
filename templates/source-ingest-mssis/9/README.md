# Source Ingest MSSIS

Ingests AIS messages from the MSSIS data provider and converts to GCI+ `MaritimeContact` messages.

## Features

- Ingests AIS messages from MSSIS data provider via socket
- Parses MSSIS specific information (e.g. timestamp)
- Decodes the following AIS message types :
  - Type 1 - 3 (Class A)
  - Type 5 (Class A static/voyage information)
  - Type 18 and 19 (Class B)
  - Type 24 (Class B static/voyage information, both formats A and B)

## Release Notes

- upgraded ingest-socket to 4.2.1

    - Fixed byte filtering to handle `\` characters correctly
    - Added content to README.md
    - MESSAGE_START_TOKENS defaults now defined in camel.properties
    - MESSAGE_END_TOKENS defaults now defined in camel.properties
    
- removed default env settings in docker-compose.yml that are identical to defaults defined in Dockerfile for
services

 
 