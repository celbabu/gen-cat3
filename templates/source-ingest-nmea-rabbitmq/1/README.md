# Source Ingest NMEA RabbitMQ

Ingests NMEA wrapped AIS messages and converts to GCI+ `MaritimeContact` messages.
 
## Features

- Consumes NMEA v4 AIS messages from a remote RabbitMQ broker
- Decodes NMEA v4 wrapper
- Decodes AIS and generates MaritimeContacts
  - Type 1 - 3 (Class A)
  - Type 5 (Class A static/voyage information)
  - Type 18 and 19 (Class B)
  - Type 24 (Class B static/voyage information, both formats A and B)

## Release Notes

- updated kstreams-microservice dependency which fixes the idle/dead state error (see known issues 1.0.0)


 
 