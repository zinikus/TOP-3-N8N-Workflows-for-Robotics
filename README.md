# Top 3 n8n Workflows for Robotics

This repository provides three ready-to-import **n8n** workflows tailored for robotics:
1. **Sensors:** MQTT ingest → threshold alert → InfluxDB write → Telegram alert
2. **Data Visualizations:** Webhook → InfluxDB → Grafana annotation
3. **Motor Control:** Webhook → MQTT publish (robot listens on `robot/motor/cmd`)

Each folder contains a workflow `.json` and a README with setup steps.

**Author:** ZINIKUS
