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

- initial release

known issues :

- use kstreams-microservice which will go into an idle/dead state (kstreams threads) if topic(s) referred to by KAFKA_INPUT_TOPICS have not been   
  created prior to starting the service



 
 