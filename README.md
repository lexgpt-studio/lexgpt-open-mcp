# LexGPT Open personal-assistant package

This package connects a compatible personal assistant to the account-authorized LexGPT Open workspace: process-linked tasks, supplied deadlines, communications, personal reminders, integration status and prepared private case-file evidence. LexGPT Conecte is the separate public jurisprudence and legislation research MCP. Neither package replaces the other.

## Connect

The hosted Streamable HTTP endpoint is `https://open.lexgpt.com.br/mcp`. OAuth discovery/DCR opens native Open sign-in and consent. Choose the account and review scopes. Revoke from Integrações → Assistentes conectados. Connections retain the originating login session's authority; reconnect when it expires or when requesting new scopes. Never put a password, client secret or provider token into these files.

`mcp.json` is the OpenAI/Dot package connection, with the official vendor authentication extension. `.mcp.json` and `.claude-plugin/plugin.json` provide the Claude bundle. Both share portable skills. Dot/Claude Duet availability depends on the platform account and supported plugin flow; an MCP endpoint or uploaded ZIP alone does not establish platform compatibility or store publication.

## Build

From this package directory, build the OpenAI ZIP with `uv run --no-project --python 3.13 python -m zipfile -c /tmp/lexgpt-open-openai.zip plugin.json mcp.json assets skills`. It must expose those inputs at its root. The Claude public repository contains this package directory's contents, including the hidden Claude manifest and `.mcp.json`, without the private application repository, runtime configuration, reviewer credentials or customer records.

The manifests own version, listing metadata and review cases. The shared skills describe the work and evidence contracts. The [Open presentation](https://lexgpt.com.br/open#mcp) explains the service and connection entry point. The copied OPEN marks come from `frontend/src/lib/open-mark.svg`; the light variant reverses the same two canonical colors. Their source font license is included. Publishing this connector package does not select a license or publish the private Open application source.

## Submit and verify

Use the [OpenAI submission portal](https://platform.openai.com/plugins) and [Claude directory submission portal](https://claude.ai/directory/manage). Before submitting, deploy the exact reviewed public HTTPS runtime, prove domain ownership as the portal requests, verify the account-bound consent flow and provide a dedicated synthetic reviewer account. Execute the positive and negative review cases from `plugin.json` against that dataset. Supply a real reviewer-accessible walkthrough URL through the portal; do not invent one in the manifest. Reviewer credentials remain in the portal's private fields and operator secret storage.

The review dataset needs an account and a process named “MCP Open” with a prepared synthetic PDF, a proposed supplied deadline, a task and a communication. Isolate it from customer accounts and external delivery destinations. Provision reviewer access through supported account/membership operations, never by borrowing an owner's session or weakening eligibility. Record the exact submitted package digest, portal ID, scan/review state and eventual published listing URL. Upload, submission, approval and publication are distinct states. Do not announce store availability until the listing is actually published.
