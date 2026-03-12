```mermaid

graph TD

User --> CDN

CDN --> API_Gateway

API_Gateway --> Product_Service
API_Gateway --> Cart_Service
API_Gateway --> Order_Service
API_Gateway --> User_Service

Product_Service --> Search_Service
Search_Service --> Elasticsearch

Order_Service --> Payment_Service
Order_Service --> Inventory_Service

Inventory_Service --> Database
