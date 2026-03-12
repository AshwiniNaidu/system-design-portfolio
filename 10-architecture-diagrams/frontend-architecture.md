```mermaid

graph TD

User --> CDN

CDN --> App_Shell

App_Shell --> Accounts_Microfrontend
App_Shell --> Payments_Microfrontend
App_Shell --> Dashboard_Microfrontend

Accounts_Microfrontend --> Shared_UI
Payments_Microfrontend --> Shared_UI
Dashboard_Microfrontend --> Shared_UI

Shared_UI --> Design_System
