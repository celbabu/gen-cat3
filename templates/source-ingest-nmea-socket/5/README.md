# Source Ingest NMEA Socket

Ingests NMEA wrapped AIS messages and converts to GCI+ `MaritimeContact` messages.
 
## Features

- Consumes NMEA v4 AIS messages from a socket (local or remote)
- Decodes NMEA v4 wrapper
- Decodes AIS and generates MaritimeContacts
  - Type 1 - 3 (Class A)
  - Type 5 (Class A static/voyage information)
  - Type 18 and 19 (Class B)
  - Type 24 (Class B static/voyage information, both formats A and B)

## Release Notes

- changed default environment variable settings in catalog
    
    - changed; REPLACEMENT_CHARACTER_ENABLED: false
    - changed; BYTE_FILTERING_ENABLED: false
    - added; USE_CLASSPATH_RESOURCE_CAMEL_PROPERTIES: true
    - added; MONITORING_HEALTHCHECK_ROUTE_ERROR_UNHEALTHY_STATE_TIMEOUT_MS: 5000
    - added; MONITORING_HEALTHCHECK_INACTIVITY_TIMEOUT_MS: 300000
     
- upgrade ingest-socket to 4.2.0
    
    - added inactivity health check
    - now automatically includes MESSAGE_START_TOKENS and MESSAGE_END_TOKENS in ALLOWABLE_CHARACTERS
    - camel.properties now extracted to root of distribution
    - ALLOWABLE_CHARACTERS and REPLACEMENT_CHARACTER now defined in camel.properties; can still override as env
      settings or via camel.properties in container
    - added DECODER_MAX_FRAME_SIZE for frame based decoding
    - frame based decoder now throws exception when DECODER_MAX_FRAME_SIZE exceeded
    - DECODER_MAX_LINE_LENGTH default now 1 MB
    
- upgraded decoded-nmea

    - upgrade ais-decoder to 4.0.4 (minor fixes; dependency updates)
    - build.gradle now uses ~/.gradle/gradle.properties for defaults
    - fixed docker image version in .gitlab-ci.yml




 
 