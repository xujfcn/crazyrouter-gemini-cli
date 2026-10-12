# Gemini CLI with Crazyrouter

Updated 2026-10-12. Gemini CLI uses the Gemini native protocol. An OpenAI `/v1` configuration is not interchangeable with this setup.

## Install and configure

Requires Node.js 20 or later. Create a key in the [Crazyrouter console](https://crazyrouter.com/console/token).

```bash
npm install -g @google/gemini-cli@0.63.0
export GEMINI_API_KEY="YOUR_CRAZYROUTER_API_KEY"
export GOOGLE_GEMINI_BASE_URL="https://api.crazyrouter.com"
export GEMINI_MODEL="gemini-3.1-pro"
gemini --model gemini-3.1-pro
```

In the authentication selector choose **Use Gemini API key**. If a saved Google OAuth login is selected, switch authentication mode before testing the gateway.

PowerShell:

```powershell
$env:GEMINI_API_KEY="YOUR_CRAZYROUTER_API_KEY"
$env:GOOGLE_GEMINI_BASE_URL="https://api.crazyrouter.com"
$env:GEMINI_MODEL="gemini-3.1-pro"
gemini --model gemini-3.1-pro
```

The API key is sent to the configured API server for authentication. Do not commit it. For persistence, follow the CLI's documented environment/configuration loading rules.

## Scope and troubleshooting

- Use Gemini models with a Gemini-native endpoint. A shared gateway key does not make Claude/GPT work inside Gemini CLI.
- `GEMINI_API_BASE` is not the documented override. Use `GOOGLE_GEMINI_BASE_URL` without `/v1` or tracking parameters.
- HTTP 401/403: verify the key, selected authentication mode and permissions. HTTP 404: verify the exact model ID and API path.
- Pricing, limits and context sizes depend on the selected model and account. There is no universal discount or unlimited quota.
- This guide pins an installation version; a complete interactive CLI/tool-use session has not been tested on every OS.

[Official configuration](https://github.com/google-gemini/gemini-cli/blob/main/docs/reference/configuration.md) · [Crazyrouter Gemini guide](https://docs.crazyrouter.com/en/integrations/gemini-cli) · [Current prices](https://crazyrouter.com/en/pricing)
