# Design Uber

## Requirements

* rider requests
* driver matching
* live tracking
* payments

## Architecture

Client → API Gateway

Services:

* rider service
* driver service
* matching service
* location service

## Technologies

Redis (location caching)

Kafka (events)

PostgreSQL (transactions)

## Architectural Diagram

```mermaid

graph TD

RiderApp --> API_Gateway
DriverApp --> API_Gateway

API_Gateway --> LocationService
API_Gateway --> MatchingService

LocationService --> Redis_Geo

MatchingService --> DriverDB

MatchingService --> TripService

TripService --> PaymentService
