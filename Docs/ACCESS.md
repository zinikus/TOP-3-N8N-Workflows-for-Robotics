# How to Import & Use in n8n

## Import
1. Open n8n → **Workflows** → **Import from File**.
2. Select the `.json` file from the relevant folder (`workflows/...`).

## Credentials / Env
- **MQTT:** broker URL, username/password or certs.
- **InfluxDB:** set env vars in n8n (`INFLUX_URL`, `INFLUX_ORG`, `INFLUX_BUCKET`, `INFLUX_TOKEN`).
- **Grafana:** API key with permissions.
- **Telegram:** Bot token + chat ID.

## Test
- Use the **Test URL** of the webhook nodes during development. Switch to **Production URL** for live usage.
