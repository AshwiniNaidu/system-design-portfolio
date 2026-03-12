# System Design Framework

Every system design should follow this structure.

## 1 Problem Statement

Clarify the system you are designing.

Example:
Design a scalable messaging platform.

## 2 Functional Requirements

* Send messages
* Receive messages
* Message history
* Notifications

## 3 Non Functional Requirements

* High availability
* Low latency
* Scalability
* Security

## 4 Capacity Estimation

Example:

Users = 10M
Messages per day = 100M

Estimate:

* storage
* bandwidth
* QPS

## 5 High Level Architecture

Client → CDN → API Gateway → Services → Database

## 6 Services Breakdown

Examples:

* Auth service
* Message service
* Notification service

## 7 Data Model

Define core tables / documents.

## 8 Scaling Strategy

* horizontal scaling
* caching
* sharding

## 9 Failure Handling

* retries
* circuit breakers
* fallbacks

## 10 Security

* authentication
* authorization
* encryption

## 11 Tradeoffs

Example:

SQL vs NoSQL
Consistency vs Availability
