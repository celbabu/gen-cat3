# Ingest Pal (development)

Ingests Pal data from the Pal SOAP based web service and converts the XML responses into GCI+ `MaritimeContacts`.

## Features

- Connects to Pal SOAP Web Service
- Requests ship position data from web service.
- Converts responses into PalMaritimeContacts and GCI+ MaritimeContacts.

## Release Notes

- Updated to add extra datetime format to handle both slashes and dashes that separate the date portion.