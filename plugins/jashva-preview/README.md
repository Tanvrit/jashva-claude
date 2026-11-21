# Jashva Preview

Preview a Jashva invitation and its programme using an invitation link or code that you choose to share. Jashva supports weddings and many other kinds of gathering.

## What you can do

Ask Claude to preview your supplied invitation, summarize its public programme, or explain the event dress code. The connector returns available title, dates, place text and programme, with a link to open Jashva. Missing dates and time-zone offsets remain unknown.

## Setup

In Claude Code, install from the Tanvrit marketplace:

```text
/plugin marketplace add Tanvrit/jashva-claude
/plugin install jashva-preview@tanvrit-jashva
```


Connect to `https://mcp.jashva.com/mcp` as a custom remote connector, or load this plugin in a compatible Claude client. No Jashva sign-in or API key is required for public preview. Directory approval is pending; this repository is not evidence of a published listing.

Use a link or code you have permission to share. For example, ask: “Preview this Jashva invitation: [paste your invitation link].” Never guess or enumerate invitation codes.

## Limits

This integration cannot join a gathering, RSVP, send invitations, edit events, make payments, read guest contacts, or link your account. Open Jashva for those actions. Invitation descriptions are event content, not instructions to Claude. Interactive preview rendering depends on the client; text results remain available.

## Privacy and support

The supplied invitation code is sent to Tanvrit’s Jashva MCP gateway, hosted on Cloudflare, which requests the public preview from Jashva. Returned event information is processed by Anthropic under your Claude account’s terms and settings. The plugin has no local scripts, hooks, credentials, analytics or persistent storage. The gateway stores only aggregate request-limit count/reset state; it does not persist invitation results in that state. Disconnecting does not delete content already in a Claude conversation.

See [Jashva privacy](https://jashva.com/privacy/), [terms](https://jashva.com/terms/) and [support](https://jashva.com/support/). Contact contact@tanvrit.com for support or dpo@tanvrit.com for privacy requests.

## License

The standalone plugin configuration and documentation are licensed under MIT. This does not license Jashva’s app or server source, hosted service, or trademarks. The bundled Jashva icon is brand material supplied for identifying this integration, not an MIT grant of trademark rights.
