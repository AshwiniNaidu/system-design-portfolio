# Metrics

Metrics help monitor system performance.

Examples:

Request latency
Error rate
CPU usage

## Tools

Prometheus
Grafana


```mermaid

graph TD

Application --> Logging_Service
Application --> Metrics_Service
Application --> Tracing_Service

Logging_Service --> Log_Storage

Metrics_Service --> Prometheus

Prometheus --> Grafana

Tracing_Service --> Jaeger
