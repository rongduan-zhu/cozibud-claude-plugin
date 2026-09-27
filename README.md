# Cozibud assistant connector

Connect Claude or Cursor to an adult caregiver's hosted Cozibud care log through its declared remote MCP server. The plugin includes one caregiver guidance skill and connects only to the declared Cozibud MCP endpoint. It runs no local code and contains no credentials.

Cozibud can read and record household care such as sleep, feeding, diapers, pumping, activities, growth and temperature. Medication and symptom records are not available through assistant connections. The service is for parents and other adult caregivers, not children. It is a recordkeeping service, not a medical device, source of medical advice, or emergency service.

## Install in Claude Code

```text
/plugin marketplace add rongduan-zhu/cozibud-claude-plugin
/plugin install cozibud@cozibud-plugins
```

Complete Cozibud sign-in and consent when prompted. Grant only the household and permissions you intend to use. You can revoke an assistant connection in Cozibud settings.

## Install in Cursor

Install Cozibud from the Cursor Marketplace, then complete Cozibud sign-in and consent when prompted. The Cursor plugin lives at `plugins/cozibud` in this repository; its manifest and MCP connection are in `.cursor-plugin/plugin.json` and `mcp.json` within that directory.

- Privacy: https://cozibud.com/privacy
- Documentation: https://docs.cozibud.com/connect-assistants
- Terms: https://cozibud.com/terms
- Support: https://cozibud.com/support

Version 0.3.0 of this connector package is licensed under Apache 2.0; see LICENSE and NOTICE. The Cozibud hosted service and private application code are not part of this repository. Earlier published versions retain the license distributed with them.
