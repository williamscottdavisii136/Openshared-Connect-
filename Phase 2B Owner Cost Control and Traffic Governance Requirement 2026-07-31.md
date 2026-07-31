# Phase 2B Owner Cost Control and Traffic Governance Requirement

Date: 2026-07-31
Repository role: public-safe connector handoff record
Issue lane: Phase 2B Device Environment Profiles / network architecture

## Owner statement

The owner states that the approved hardware, computers, phones, local devices, and private home-network environment are owner-controlled. The owner also states that outbound network traffic, internet usage, cloud usage, provider calls, subscription usage, token usage, quota usage, hosted-code usage, and other metered activity must be subject to owner governance.

## Controlling rule

Approved devices and applications on the owner-controlled R&D network must not be allowed to create unauthorized or unapproved cost, billing, quota, token, subscription, hosted-compute, cloud-storage, connector, plugin, marketplace, or provider-control-plane activity.

The owner-controlled network may enforce cost governance through lawful local controls, including:

- allow / deny routing policy;
- VLAN and subnet segmentation;
- firewall policy;
- DNS policy;
- proxy policy;
- application allowlists and blocklists;
- approved-node gating;
- approved-provider gating;
- metered-route classification;
- cost-unknown quarantine;
- owner-approval prompts or receipts;
- local/offline/BYOK/MCP routing where lawful and authorized;
- logging that avoids raw secrets and private identifiers.

## Required classification

Each relevant application, program, app, node, agent, chatbot, terminal process, browser process, mobile app, IDE process, connector, plugin, or service client must be classified for whether it attempts to use:

- ordinary internet access;
- local-only access;
- offline/local model access;
- BYOK access;
- MCP access;
- provider API access;
- hosted code execution;
- cloud storage;
- token or quota ledger;
- subscription or seat entitlement;
- app-store / marketplace entitlement;
- model-specific paid access;
- connector or plugin metering;
- bandwidth-heavy sync, upload, backup, indexing, OCR, transcription, embedding, vectorization, or analysis.

## Cost-control policy

Unknown cost is not approved cost.

Unknown entitlement is not approved entitlement.

Unknown subscription status is not approved subscription use.

Unknown token/quota behavior is not approved token/quota use.

Any route that may increase the owner’s internet bill, provider bill, subscription bill, cloud bill, hosted-compute bill, token/quota usage, or other metered charge must be classified before approval.

## Network boundary

The owner-controlled protected R&D network is not public access. Non-owner household devices and guests are not authorized R&D subnet participants. VLAN and subnet segmentation remain controlling security layers.

## Negative boundary

This record does not authorize:

- provider-billing circumvention;
- subscription circumvention;
- token/quota/rate-limit evasion;
- unauthorized credential use;
- session capture;
- certificate forgery;
- unauthorized third-party access;
- public interception;
- unauthorized network access.

The valid control is owner-side traffic governance: block, allow, route, classify, approve, deny, quarantine, simulate lab responses where lawful, and preserve public-safe receipts.

## Public-safe publication note

This public record intentionally omits private network names, IP addresses, MAC addresses, serial numbers, IMEIs, hostnames, local account details, credentials, passwords, keys, tokens, certificates, cookies, sessions, and raw billing artifacts.
