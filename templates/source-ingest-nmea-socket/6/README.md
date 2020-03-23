# Source Ingest NMEA Socket

Ingests NMEA wrapped AIS messages and converts to GCI+ `MaritimeContact` messages.
 
## Features

- Consumes NMEA v4 AIS messages from a socket (local or remote)
- Decodes NMEA v4 wrapper
- Decodes AIS and generates MaritimeContacts
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




 
 