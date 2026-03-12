# Design Amazon

## Core Services

* product catalog
* search
* cart
* checkout
* payments
* order management

## Architecture

User → CDN → API Gateway

Services:

Product service
Search service
Cart service
Order service

## Data Storage

Products → NoSQL
Orders → SQL
Search → Elasticsearch

## Architectural diagram

```mermaid

graph TD

User --> CDN
CDN --> API_Gateway

API_Gateway --> ProductService
API_Gateway --> CartService
API_Gateway --> OrderService

OrderService --> PaymentService
OrderService --> InventoryService

OrderService --> EventBus

EventBus --> ShippingService
EventBus --> NotificationService
