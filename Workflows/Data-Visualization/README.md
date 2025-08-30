# Data Visualizations: Webhook → InfluxDB → Grafana Annotation

**Level:** Intermediate  
Accepts POSTed samples, writes them to **InfluxDB**, and creates a **Grafana** dashboard annotation for quick visual context.

## Quick Start
1. Set env vars: `INFLUX_URL`, `INFLUX_ORG`, `INFLUX_BUCKET`, `INFLUX_TOKEN`.
2. Add **Grafana** credentials (API key).
3. Import the JSON and copy the **production webhook URL** into your data source or script.

## Example Request
```bash
curl -X POST $WEBHOOK_URL -H "Content-Type: application/json"   -d '{ "sensor":"humidity", "value":55, "unit":"%" }'
```
---
