# Cozibud for Claude

This plugin connects Claude to the hosted Cozibud MCP service. It is for parents and other adult caregivers; it is not intended for use by children.

The plugin includes one guidance skill and the declared remote MCP connection at https://cozibud.com/api/mcp. It runs no local code. Claude and the Cozibud authorization service handle OAuth sign-in and consent; no credentials are bundled with the plugin. After consent, the service reads and stores care records for the selected household according to the granted permissions. It retains records while the account exists, subject to the deletion process in the privacy policy.

Cozibud can read and record sleep, feeding, diapers, pumping, activities, growth and temperature. Medication and symptom records are not exposed through assistant connections. Cozibud is a recordkeeping service, not a medical device, source of medical advice, or emergency service.

## Test locally

1. Run `claude plugin validate ./plugins/cozibud --strict`.
2. Start Claude Code with `claude --plugin-dir ./plugins/cozibud`.
3. Open `/mcp` and complete Cozibud sign-in and consent.
4. Try a synthetic household first, for example: “What was the most recent feed?”

- Documentation: https://docs.cozibud.com/connect-assistants
- Privacy: https://cozibud.com/privacy
- Terms: https://cozibud.com/terms
- Support: https://cozibud.com/support

License: see LICENSE in this plugin folder. Earlier published versions retain their original license.
