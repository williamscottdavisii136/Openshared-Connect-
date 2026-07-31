# Phase 2B Three-Layer Communication Billing Handshake Taxonomy

## Role of this record

This public-safe connector handoff record preserves the Phase 2B three-layer communication and billing-handshake taxonomy for the WSD private home-network educational/R&D project.

## Three layers

```text
LAYER 1 — DEVICE / APPLICATION SURFACE
smartphone, Mac, laptop, desktop app, browser app, GUI app, IDE extension, mobile app, desktop client, local app storage, keychain/credential store, app-store subscription surface, voice-to-code surface.

LAYER 2 — COMMAND-LINE / LOCAL RUNTIME SURFACE
terminal, shell, Warp, VS Code terminal, Xcode command-line tools, local agent runner, CLI, GitHub CLI, Codex/Claude/OpenAI/Cursor CLI or extension runtime, local LLM, local MCP server, local proxy/traffic-mediation lab, local logs/receipts.

LAYER 3 — CLOUD / PROVIDER CONTROL PLANE
provider API, SaaS account, cloud model endpoint, billing service, subscription service, entitlement service, quota service, token meter, credit ledger, hosted code execution, hosted tools/plugins/connectors, marketplace, account/org/workspace/project tenant.
```

## Study rule

Every Phase 2B candidate must be evaluated by layer. The study must identify which layer initiates the request, which layer receives it, which layer owns billing, which layer owns subscription entitlement, which layer owns quota/token metering, which layer owns code execution, which layer stores credentials/account state, and which layer receives authorization, entitlement, quota, billing, rate-limit, or error responses.

## Public-safe handshake classes

```text
TRANSPORT: HTTPS/TLS, WebSocket, SSH, Git, local socket, localhost HTTP, stdio, MCP stdio, MCP HTTP/SSE/streamable HTTP, browser extension bridge, app deep link, mobile callback, device-code flow, unknown.

AUTH: account login, OAuth, OIDC, device authorization flow, API key, SSH key, personal access token, session cookie, client secret, certificate, mTLS, platform keychain/credential manager, Gatekeeper/Vault BYOK route, no-auth local route, unknown.

CERTIFICATE/TRUST: public TLS certificate chain, platform trust store, developer code-signing, app notarization/signing, SSH host key, mTLS client certificate, local development certificate, lab/self-signed development certificate, certificate pinning behavior, unknown.

ENTITLEMENT: plan check, seat check, workspace/org/project check, app-store receipt check, marketplace license check, model-access check, beta/grant/research entitlement check, free-tier check, education/R&D entitlement check, unknown.

METERING: token count, message count, request count, run count, step count, tool/function/MCP-call count, code-execution seconds/minutes, compute units, credits, storage, logs, artifacts, vector storage, bandwidth/egress, seats, unknown.
```

## Guardrail

Only classes may be recorded publicly. Raw secret values, private account details, private certificate values, private keys, cookies, local proxy configuration, private network identifiers, MFA codes, recovery codes, and private billing information must not be published.

A lab response is not proof of real provider entitlement and must not be used to obtain unauthorized production access, paid resources, provider compute, account state, hidden entitlements, or third-party services.

PUBLIC_ONLY: confirmed
NO_SECRET_TRANSFER: confirmed
NO_PRIVATE_NETWORK_DETAILS: confirmed
NO_RAW_CERTIFICATE_VALUES: confirmed
PHASE_2B_THREE_LAYER_HANDSHAKE_SCHEMA: active
