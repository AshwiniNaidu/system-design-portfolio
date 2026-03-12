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
