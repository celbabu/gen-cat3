# Ingest Pal (development)

Ingests Pal data from the Pal SOAP based web service and converts the XML responses into GCI+ `MaritimeContacts`.

## Features

- Connects to Pal SOAP Web Service
- Requests ship position data from web service.
- Converts responses into PalMaritimeContacts and GCI+ MaritimeContacts.

## Release Notes

- Added new kafka topic for GetNav.  Aircraft MaritimeContacts now to to their own topic.