# SaaS Architecture Diagram

```mermaid
graph TD

User --> CDN
CDN --> API

API --> Auth
API --> Billing
API --> Analytics

Analytics --> Kafka
Kafka --> Warehouse
```
