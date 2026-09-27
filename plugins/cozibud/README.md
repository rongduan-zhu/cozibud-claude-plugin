# Cozibud for Claude and Cursor

This plugin connects Claude or Cursor to the hosted Cozibud MCP service. It is for parents and other adult caregivers; it is not intended for use by children.

The plugin includes one guidance skill and a declared remote MCP connection for each supported client. It runs no local code. The client and the Cozibud authorization service handle OAuth sign-in and consent; no credentials are bundled with the plugin. After consent, the service reads and stores care records for the selected household according to the granted permissions. It retains records while the account exists, subject to the deletion process in the privacy policy.

Cozibud can read and record sleep, feeding, diapers, pumping, activities, growth and temperature. Medication and symptom records are not exposed through assistant connections. Cozibud is a recordkeeping service, not a medical device, source of medical advice, or emergency service.

## Test locally

1. Run `claude plugin validate ./plugins/cozibud --strict`.
2. Start Claude Code with `claude --plugin-dir ./plugins/cozibud`.
3. Open `/mcp` and complete Cozibud sign-in and consent.
4. Try a synthetic household first, for example: “What was the most recent feed?”

For Cursor, install the plugin from the Marketplace and complete OAuth sign-in. Confirm that its Cozibud MCP server and caregiver skill appear in Cursor before testing with a synthetic household.

- Privacy: https://cozibud.com/privacy
- Documentation: https://docs.cozibud.com/connect-assistants
- Terms: https://cozibud.com/terms
- Support: https://cozibud.com/support

License: Apache-2.0; see LICENSE in this plugin folder and NOTICE in the repository root. Earlier published versions retain the license distributed with them.
