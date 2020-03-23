# Ingest Pal (1.0.5)

Ingests Pal data from the Pal SOAP based web service and converts the XML responses into GCI+ `MaritimeContacts`.

## Features

- Connects to Pal SOAP Web Service
- Requests ship position data from web service.
- Converts responses into PalMaritimeContacts and GCI+ MaritimeContacts.
    
## Release Notes

- Added prometheus java agent to dockerfile java_opts env variable.
- Updated to first get flag from mmsi then try from country field.
    - Uses fuzzy matcher to match country code when retrieving from country field.