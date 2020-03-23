# Ingest Innav (1.0.3)

Ingests Innav data from the Innav SOAP based web service and converts the XML responses into GCI+ `MaritimeContacts`.

## Features

- Connected to Innav SOAP Web Service
- Requests ship position data from web service.
- Converts responses into InnavMaritimeContacts and GCI+ MaritimeContacts.
    
## Release Notes

- Added prometheus java agent to dockerfile java_opts env variable.