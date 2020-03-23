# Ingest Innav (1.0.2)

Ingests Innav data from the Innav SOAP based web service and converts the XML responses into GCI+ `MaritimeContacts`.

## Features

- Connected to Innav SOAP Web Service
- Requests ship position data from web service.
- Converts responses into InnavMaritimeContacts and GCI+ MaritimeContacts.
    
## Release Notes

- Updated to use avro-validator 1.1.1 which fixes heading 511 (heading unavailable) error.