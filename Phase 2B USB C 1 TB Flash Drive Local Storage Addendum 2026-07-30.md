# Phase 2B USB-C 1 TB Flash Drive Local Storage Addendum 2026-07-30

## Public-safe handoff summary

This addendum records one owner-provided USB-C 1 TB flash drive as a local removable-storage device in the Phase 2B three-layer communication, billing, request, reply, and storage taxonomy.

```text
STORAGE PROFILE: USB-C connector flash drive
CAPACITY: 1 TB, owner-stated
DEVICE CLASS: local removable storage
NETWORK STATUS: not independently a network node unless mounted by an owner-controlled host and shared through an authorized route
```

## Routing rule

The drive is local storage by default. It becomes network-relevant only if an owner-controlled host device mounts it and shares it through an authorized Wi-Fi, SSH, Bluetooth, local file-sharing, MCP, terminal, or other owner-approved route.

## Billing rule

```text
Local removable storage is not cloud billing by itself.
Local removable storage is not AI-provider billing authorization.
Local removable storage is not subscription authorization.
Local removable storage is not token/quota authorization.
Cloud/provider billing may become involved only if an application syncs, uploads, backs up, indexes, scans, processes, embeds, vectorizes, or otherwise sends drive contents to a provider-controlled service.
```

## Guardrail

No storage serials, UUIDs, encryption keys, passwords, private file names, private file contents, raw credentials, token values, certificate values, cookies, session material, recovery codes, MFA codes, or operational secrets are included.

PUBLIC_ONLY: confirmed
NO_SECRET_TRANSFER: confirmed
NO_PRIVATE_FILE_CONTENTS: confirmed
PHASE_2B_USB_C_1TB_STORAGE_PROFILE: active
