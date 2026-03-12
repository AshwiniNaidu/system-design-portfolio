# Design WhatsApp

## Functional Requirements

* send messages
* receive messages
* group chat
* message history
* read receipts

## Non Functional Requirements

* low latency
* high availability
* real-time communication

## Architecture

Client → WebSocket Gateway → Messaging Service → Message Queue → Storage

## Key Components

WebSocket servers
Message queue (Kafka)
Message storage (NoSQL)

## Scaling

* WebSocket clusters
* Redis pub/sub
* horizontal scaling

## Architectural diagram

```mermaid

graph TD

User --> LoadBalancer

LoadBalancer --> WebSocketServer1
LoadBalancer --> WebSocketServer2

WebSocketServer1 --> MessagingService
WebSocketServer2 --> MessagingService

MessagingService --> Kafka

Kafka --> MessageStorage
Kafka --> NotificationService

MessageStorage --> NoSQLDB
