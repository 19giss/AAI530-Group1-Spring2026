# Conceptual IoT System Diagram (Smart City Traffic Forecasting)

```mermaid
flowchart LR
  A[Roadway Traffic Sensors\n(loop detectors / roadside sensors)] --> B[Edge Gateway\naggregation + validation]
  B --> C[Network Transport\ncellular/fiber; MQTT/HTTPS]
  C --> D[Cloud / Central Platform\nstorage + preprocessing]
  D --> E[Analytics + ML Pipeline\nbaseline + LSTM forecasting]
  E --> F[Decision Support Layer\nTableau Dashboard + reports]
  F --> G[Users\nTraffic operators + planners]
