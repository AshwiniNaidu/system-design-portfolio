```mermaid

graph TD

Service_A --> Event_Bus

Event_Bus --> Service_B
Event_Bus --> Service_C
Event_Bus --> Service_D

Service_B --> Database

Service_C --> Cache

Service_D --> Analytics
