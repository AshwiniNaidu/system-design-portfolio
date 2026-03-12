# Design Google Docs

## Requirements

* collaborative editing
* version history
* document storage

## Architecture

Client → WebSocket → Collaboration Service

## Key Concepts

Operational transformation
real-time synchronization

##Architectural Diagram

```mermaid

graph TD

User --> WebSocketGateway

WebSocketGateway --> CollaborationService

CollaborationService --> OperationalTransform

OperationalTransform --> DocumentStorage

DocumentStorage --> VersionHistory
