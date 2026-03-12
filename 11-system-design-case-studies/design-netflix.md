# Design Netflix

## Requirements

* video streaming
* recommendation engine
* user profiles
* content catalog

## Architecture

User → CDN → API Gateway → Microservices

Services:

* video service
* recommendation service
* user service

## Key Concepts

CDN caching
adaptive bitrate streaming
microservices
