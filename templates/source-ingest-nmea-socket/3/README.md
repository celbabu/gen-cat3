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

- updated to ais-decoder 4.0.3 to fix lat / lon validation and add cargo descriptions to MaritimeContacts





 
 