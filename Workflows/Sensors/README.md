# Sensors: MQTT Ingest → InfluxDB + Telegram Alert

**Level:** Intermediate  
This workflow subscribes to `robot/sensors/#` via **MQTT Trigger**, checks a threshold, writes data to **InfluxDB** (HTTP API), and sends a Telegram alert when values exceed the threshold.

## Quick Start
1. Add **MQTT Trigger** credentials (broker URL, topic).
2. Set env vars in n8n: `INFLUX_URL`, `INFLUX_ORG`, `INFLUX_BUCKET`, `INFLUX_TOKEN`.
3. Add **Telegram** credentials (bot token, chat ID).
4. Import the JSON in this folder into n8n.

## Expected Payload
```json
{ "sensor": "temp", "value": 32.5, "unit": "C" }
```

## Notes
- InfluxDB write uses line protocol via HTTP. You can swap this for the community **InfluxDB node** if installed.
