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
