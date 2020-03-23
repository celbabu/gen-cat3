# Vessel Identity Image

This service provides a lits of image URLs for a given vessel imo

## Features
 - client sends request(imo) to Vessel Identity Image service
 - The service validates the imo and returns error response in case of an error, otherwise prepares a query for the backend JDBC datasource
 - backend returns a list of images
 - The service prepares image urls based on the list and then return them to the client.
   
## Release Notes

  - version: n/a


