# Ingest-Mssis (development)

Ingest Mssis is a microservice that replaces the download/upload functionality of the TV32 software.

## Download Features

- Connects to VOLPE distribute server using a secure connection created using stunnel.
- Handshakes with server for authentication.
- If authentication is valid then a stream of AIS data is accessed and consumed by the microservice.
- Data consumed is then forwarded to a topic on the kafka broker.


## Upload Features

- Connects to VOLPE collector server using a secure connection created using stunnel.
- Handshakes with server for authentication.
- If authentication is valid then the stream of Coastal AIS data from the Canadian DND is accessed and uploaded to the VOLPE collector server.
    
## Release Notes

- development release