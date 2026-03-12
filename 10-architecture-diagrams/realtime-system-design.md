```mermaid

graph TD

Client --> LoadBalancer

LoadBalancer --> WebSocket_Server1
LoadBalancer --> WebSocket_Server2

WebSocket_Server1 --> Message_Service
WebSocket_Server2 --> Message_Service

Message_Service --> Kafka

Kafka --> Notification_Service
Kafka --> Storage

Storage --> Database
