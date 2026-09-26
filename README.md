# Cozibud for Claude

Connect Claude to an adult caregiver's hosted Cozibud care log through its declared remote MCP server. The plugin includes one caregiver guidance skill and connects only to https://cozibud.com/api/mcp. It runs no local code and contains no credentials.

Cozibud can read and record household care such as sleep, feeding, diapers, pumping, activities, growth and temperature. Medication and symptom records are not available through assistant connections. The service is for parents and other adult caregivers, not children. It is a recordkeeping service, not a medical device, source of medical advice, or emergency service.

## Install in Claude Code

```text
/plugin marketplace add rongduan-zhu/cozibud-claude-plugin
/plugin install cozibud@cozibud-plugins
```

Complete Cozibud sign-in and consent when prompted. Grant only the household and permissions you intend to use. You can revoke an assistant connection in Cozibud settings.

- Documentation: https://docs.cozibud.com/connect-assistants
- Privacy: https://cozibud.com/privacy
- Terms: https://cozibud.com/terms
- Support: https://cozibud.com/support

The plugin is source visible under the terms in LICENSE. Earlier published versions retain their original license.
