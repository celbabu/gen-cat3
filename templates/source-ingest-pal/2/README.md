# Ingest Pal (1.0.3)

Ingests Pal data from the Pal SOAP based web service and converts the XML responses into GCI+ `MaritimeContacts`.

## Features

- Connects to Pal SOAP Web Service
- Requests ship position data from web service.
- Converts responses into PalMaritimeContacts and GCI+ MaritimeContacts.
    
## Release Notes

- Updated to use avro-validator 1.1.1 which fixes heading 511 (heading unavailable) error.