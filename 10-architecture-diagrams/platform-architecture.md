```mermaid

graph TD

Developer --> Git_Repo

Git_Repo --> CI_CD_Pipeline

CI_CD_Pipeline --> Container_Registry

Container_Registry --> Kubernetes_Cluster

Kubernetes_Cluster --> Service_Mesh

Service_Mesh --> Observability_Stack
