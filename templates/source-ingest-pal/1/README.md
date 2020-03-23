# Ingest Pal (1.0.2)

Ingests Pal data from the Pal SOAP based web service and converts the XML responses into GCI+ `MaritimeContacts`.

## Features

- Connects to Pal SOAP Web Service
- Requests ship position data from web service.
- Converts responses into PalMaritimeContacts and GCI+ MaritimeContacts.
    
## Release Notes

- Fixed bug where category types were always set to unknown.
- Fixed bug where speed was being saved in knots instead of m/s.
- Changed dependency avro-validators to v1.1.0
- Updated kafka_serializer_class to point to correct class.
- Updated prometheus port settings.