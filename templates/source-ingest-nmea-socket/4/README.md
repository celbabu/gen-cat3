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

- upgrade ais-decoder to 4.0.4 (minor dependency updates; fixes)
- upgrade to ais-decoder to include position accuracy parsing (in translation hints)
- added optional filter (default false) for zeroed positions (e.g. at 0, 0 lat/lon)





 
 