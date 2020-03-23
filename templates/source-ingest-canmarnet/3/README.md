# Ingest Canmarnet Stack

Creates a stack containing ingest-canmarnet, decode-tca, decode-otg and docker-clamav virus scanner.

## Features

- Ingest-canmarnet
    - Consumes emails using IMAP.
    - Produces TCA, AA1, and OSWEX emails.
- Docker-ClamAV
    - Used in conjunction with ingest-canmarnet to scan all consumed emails before processing.
- Decode-tca
    - Parses and decodes TCA emails and generates MaritimeContacts.
- Decode-otg
    - Parses and decodes oswex GOLD messages and generates MaritimeContacts.
- Decode-aa1
    - Disabled for now, not receiving any AA1 messages because of external circumstances. 

## Release Notes

- initial release
 