# Cozibud for Claude Code

This community plugin connects Claude Code to the hosted Cozibud MCP service. It is for parents and other adult caregivers; it is not intended for use by children.

Cozibud can read and record household care such as sleep, feeding, diapers, pumping, activities, growth, temperature, medication, and symptoms. It is a recordkeeping service, not a medical device, source of medical advice, or emergency service.

## Test locally

1. Run `claude plugin validate ./plugins/cozibud --strict`.
2. Start Claude Code with `claude --plugin-dir ./plugins/cozibud`.
3. Open `/mcp` and complete Cozibud sign-in and consent.
4. Try a synthetic household first, for example: “What was the most recent feed?”

The plugin contains no credentials. OAuth tokens are handled by Claude Code and the Cozibud authorization service.

Documentation: https://docs.cozibud.com/connect-assistants

Support: https://cozibud.com/support
