# Motor Control: Webhook → MQTT Publish

**Level:** Intermediate  
Receives motor commands over an HTTP **Webhook**, publishes them to an **MQTT** topic (`robot/motor/cmd`), and responds with an ACK.

## Quick Start
1. Configure **MQTT** node (broker URL, authentication).
2. Import the JSON and copy the production webhook URL into your control UI.
3. Your robot subscribes to `robot/motor/cmd` and executes commands.

## Example Command
```bash
curl -X POST $WEBHOOK_URL -H "Content-Type: application/json"   -d '{ "direction":"forward", "speed":128 }'
```
---
