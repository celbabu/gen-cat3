# Vessel Identity Service

Works as a proxy to Elasticsearch. Client will use this service to search for vessels stored in Elasticsearch.

## Features

  - Client sends request to Identity service
  - The service validates the request and returns error response in case of an error, otherwise forwards the request to Elasticsearch
  - Elastcisearch returns a list of matching vessels as result.
  - The service returns the list of matching vessels to the client after calculating a match score for each vessel.
    
## Release Notes

version: 1.1.0 (updating Vessel Identity to 1.2.0)

  - swagger definition for the REST api
  - code clean up
  - bug fix: when there is no match the service was returning string(from elastcisearch) instead 0.
  - custom exception handling


