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

## Architectural diagram

```mermaid
graph TD

User --> DNS
DNS --> CDN

CDN --> EdgeCache
EdgeCache --> VideoService

VideoService --> MetadataService
VideoService --> RecommendationService

MetadataService --> CatalogDB
RecommendationService --> MLModels

VideoService --> Storage
Storage --> VideoEncodingPipeline
