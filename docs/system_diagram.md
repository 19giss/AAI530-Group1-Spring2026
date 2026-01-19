# Conceptual IoT System Diagram (Smart City Traffic Forecasting)

```mermaid
flowchart LR
  A["Roadway traffic sensors<br/>loop detectors, roadside sensors"] --> B["Edge gateway<br/>aggregation and validation"]
  B --> C["Network transport<br/>cellular or fiber, MQTT or HTTPS"]
  C --> D["Cloud or central platform<br/>storage and preprocessing"]
  D --> E["Analytics and ML pipeline<br/>baseline and LSTM forecasting"]
  E --> F["Decision support layer<br/>Tableau dashboard and reports"]
  F --> G["Users<br/>traffic operators and planners"]
