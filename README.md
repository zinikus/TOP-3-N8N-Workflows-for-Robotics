# Top 3 N8N Workflows for Robotics:

<img width="355" height="142" alt="image" src="https://github.com/user-attachments/assets/e44538f2-26d0-41ce-9fda-99309be8855d" />

This repository provides three ready-to-import **n8n** workflows tailored for robotics:
1. **Sensors:** MQTT ingest → threshold alert → InfluxDB write → Telegram alert
2. **Data Visualizations:** Webhook → InfluxDB → Grafana annotation
3. **Motor Control:** Webhook → MQTT publish (robot listens on `robot/motor/cmd`)

**Use-Cases:**
1. Real-time monitoring of robot health, safety alerts, and predictive maintenance.

2. Helps operators visualize robotic activity (missions completed, battery level changes, or faults) directly on Grafana dashboards.

3. Simple remote control system for robotic movement, testing commands, or integrating higher-level decision systems.


Each folder contains a workflow `.json` and a README with setup steps.

**Author:** @ZINIKUS (https://github.com/zinikus/)
