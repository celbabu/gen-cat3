# Ingest Pal (development)

Ingests Pal data from the Pal SOAP based web service and converts the XML responses into GCI+ `MaritimeContacts`.

## Features

- Connects to Pal SOAP Web Service
- Requests ship position data from web service.
- Converts responses into PalMaritimeContacts and GCI+ MaritimeContacts.

## Release Notes

- speed now stored in speed over ground instead of speed (e.g. e/ respect to medium)
- updated MaritimeContact etc. metadata constants to be stored in properties file instead of hardcoded.

known issues:

- metadata constants are double quoted