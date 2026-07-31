# Phase 2B VLAN Segmentation Printer MacBook Phone Isolation Addendum

Date: 2026-07-30
Repository role: Openshared public-safe connector handoff
Phase: 2B device/network environment mapping

## Owner-stated VLAN segmentation

The owner states that the protected R&D home-network environment includes separate VLAN segmentation:

- printers are on their own VLAN;
- MacBooks are on their own VLAN;
- phones are on their own VLAN.

No VLAN IDs, IP addresses, subnet masks, router addresses, MAC addresses, SSIDs, Wi-Fi passwords, SSH keys, credentials, tokens, certificates, serial numbers, IMEIs, hostnames, or local account details are included in this public connector record.

## Handoff rule

Any downstream connector, agent, chatbot, coding assistant, IDE, terminal runner, MCP route, BYOK route, or local automation must treat the VLAN arrangement as a protected R&D isolation control, not a public-access route.

## Cross-VLAN classification

Cross-VLAN access is not automatic and must be separately classified:

```text
DENIED_BY_DEFAULT
ALLOW_PRINT_ONLY
ALLOW_DISCOVERY_ONLY
ALLOW_SSH_APPROVED_NODE_ONLY
ALLOW_FILE_TRANSFER_APPROVED_NODE_ONLY
ALLOW_MCP_OR_LOCAL_AGENT_APPROVED_NODE_ONLY
ALLOW_FULL_ROUTE_APPROVED_NODE_ONLY
UNVERIFIED
```

## Security boundary

The VLAN segmentation supports:

- no public access;
- no non-owner household access;
- approved-node-only local network membership;
- approved-service-only cross-VLAN access;
- no default lateral movement between printer, MacBook, and phone classes;
- no provider entitlement assumption from local connectivity.

## Bluetooth / USB / SSH distinction

Bluetooth remains peer-to-peer / near-field local connectivity and is not VLAN membership.

USB direct-link cabling is a physical local link and is not VLAN membership by itself.

SSH is authenticated access over an authorized IP route. If SSH crosses VLANs, an explicit allowed route and authentication policy must exist.
