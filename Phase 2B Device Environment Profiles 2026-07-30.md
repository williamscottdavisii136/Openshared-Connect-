# Phase 2B Device Environment Profiles

## Role of this record

This public-safe connector handoff record adds owner-provided device-environment profiles to the Phase 2B three-layer communication, billing, handshake, certificate/trust, request, and reply taxonomy.

This record does not publish serial numbers, IMEI values, phone numbers, carrier account numbers, IP addresses, MAC addresses, private network names, private account details, raw credentials, token values, certificate values, cookies, session material, recovery codes, MFA codes, private legal materials, or operational secrets.

## Owner-provided device environment

```text
ANDROID SMARTPHONE ENVIRONMENT:
- Android smartphone label: 8:15
- Android smartphone label: A16
- Android smartphone label: 817

MAC ENVIRONMENT:
- MacBook Air, 2015, owner states running Monterey
- MacBook Pro, 2012, legacy environment, owner states Yosemite
```

The labels `8:15`, `A16`, and `817` are preserved as owner-provided labels until exact device model, Android version, vendor, and runtime profile are separately verified.

## Connector handoff rule

Future agents and connected sessions must classify these devices across:

```text
LAYER 1 — device / application surface
LAYER 2 — command-line / local runtime surface
LAYER 3 — cloud / provider control plane
```

For each AI-agent or AI-chatbot candidate, determine what device initiates the request, which layer receives the request, what handshake class is used, what credential or certificate class is involved, what billing/quota/entitlement response is expected, and whether a local/offline/MCP/BYOK/Gatekeeper-Vault route exists.

Only public-safe classes and statuses may be carried here.

Unknown device model is not approval.
Unknown OS version is not approval.
Unknown app-store or marketplace entitlement is not authorization.
Unknown cloud/provider route is not approved.
Unknown certificate/trust handshake is not approval.
Unknown token/quota/billing status is not authorization.
Unknown license status is not authorization.

PUBLIC_ONLY: confirmed
NO_SECRET_TRANSFER: confirmed
NO_PRIVATE_DEVICE_IDENTIFIERS: confirmed
PHASE_2B_DEVICE_PROFILES: active
