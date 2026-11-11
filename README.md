# Lawve for Antigravity

Use legal methods and guidance shared by practitioners directly in Antigravity.

Lawve brings together legal AI skills written by practicing lawyers, in-house counsel, academics, and legal technologists from around the world, covering a wide range of practice areas and jurisdictions. Each skill gives Antigravity step-by-step instructions for a specific legal task.

Describe your legal task, and Antigravity can find a relevant skill on Lawve and apply its author’s methodology directly to your documents or questions.

You can use the Lawve connector to:

- Challenge an argument: “Find a skill on Lawve to review this legal argument from opposing counsel’s perspective, then identify weaknesses I should address.”
- Assess an AI system: “Find and apply a skill on Lawve to help classify our recruitment AI tool under the EU AI Act and identify the obligations that follow.”
- Improve legal writing: “Use a relevant skill on Lawve to make this legal letter clearer and more persuasive, while preserving the facts and my position.”
- Review against your standards: “Find a skill on Lawve to review this supplier agreement against our negotiation playbook, then flag deviations and suggest changes.”

## Requirements

- Google Antigravity with plugin and remote MCP support.
- A Lawve account with access to the requested resources. [Create an account](https://lawve.ai/sign-up).
- Network access to `https://mcp.lawve.ai` and `https://studio.lawve.ai`.

## Install from GitHub

With the Antigravity CLI available:

```sh
agy plugin install https://github.com/lawve-ai/antigravity-plugin
```

This installs the plugin from its source repository, not from the Antigravity Marketplace. Marketplace publication is pending.

## Validate and install locally

From this repository's root, with the Antigravity CLI available:

```sh
agy plugin validate --strict .
agy plugin install .
agy plugin list --json
```

Local strict validation, installation, and a Lawve connection test have been completed by the publisher. This does not constitute Marketplace approval.

## Connect your account

Open the installed plugin's MCP connection settings and authenticate with Lawve when prompted. Complete sign-in and consent in the browser, then follow Antigravity's instructions to finish connecting.

The server supports OAuth with PKCE and Dynamic Client Registration. No shared client secret or API key is bundled with the plugin. Never paste passwords or access tokens into a conversation. If Antigravity asks you to transfer an authorization code, enter it only in its authentication interface.

The connector exposes `run_command` to navigate, search, and read authorized Lawve resources. It runs against Lawve's resource environment, not your computer's shell. Antigravity can use the retrieved methods to support your work; check their authorship, scope, jurisdiction, and applicability.

## Scope and limitations

The connection is read-only for Lawve resources: it does not publish, edit, or delete them. Resource availability depends on the catalog and your permissions. Lawve provides practitioner-authored methods and content, not legal advice. Verify applicable law, facts, sources, and generated output before relying on a result.

Other Antigravity tools have separate permissions; this connector's read-only scope does not restrict them. Installing this plugin does not include the Lawve backend or grant a license to redistribute the resource catalog.

## Troubleshooting

Check that the plugin is enabled, its MCP server is connected, and your Lawve account can access the requested resource. Reauthenticate through the MCP connection settings if prompted. Report the Antigravity version, time, failing step, and sanitized error message; never share tokens, authorization codes, passwords, or confidential documents.

## Support and policies

- [Documentation](https://lawve.ai/docs)
- [Contact Lawve](https://lawve.ai/about)
- [Privacy policy](https://lawve.ai/privacy)
- [Terms of use](https://lawve.ai/terms)
