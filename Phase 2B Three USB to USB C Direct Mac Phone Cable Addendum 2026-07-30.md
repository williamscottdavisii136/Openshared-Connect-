# Phase 2B Three USB to USB-C Direct Mac Phone Cable Addendum 2026-07-30

## Purpose

This public-safe Openshared addendum records three owner-provided direct physical cable routes between the Macintosh environment and the Samsung smartphone environment for Phase 2B handoff.

It does not publish serial numbers, phone numbers, IMEI values, MAC addresses, IP addresses, private account details, raw credentials, token values, certificate values, cookies, session material, recovery codes, MFA codes, private network names, private legal materials, or operational secrets.

## Public-safe physical link profile

```text
CABLE GROUP: three direct Mac-to-phone cables
CABLE TYPE: USB connector on Mac side and USB-C connector on Samsung phone side, owner-stated
COUNT: 3 cables
ASSIGNMENT: one cable for each Mac profile
FUNCTION: direct physical Mac-to-Samsung-phone connection
```

## Public-safe host mapping

```text
MAC CABLE ROUTE 1: MacBook Air 2015 Monterey profile to Samsung phone profile through direct USB/USB-C cable
MAC CABLE ROUTE 2: MacBook Air 2015 secondary profile to Samsung phone profile through direct USB/USB-C cable
MAC CABLE ROUTE 3: MacBook Pro 2012 Yosemite profile to Samsung phone profile through direct USB/USB-C cable
```

## Phase 2B handshake significance

Each cable route must classify the actual negotiated mode:

```text
charging-only;
file transfer / MTP;
photo transfer / PTP;
USB tethering;
ADB / debugging, only if owner-authorized and enabled;
USB accessory mode;
local backup / restore;
local media import;
local device trust prompt;
unknown.
```

## Billing and authorization consequence

A physical cable is not cloud billing, AI-provider authorization, subscription authorization, token/quota authorization, credential-transfer authorization, or certificate-transfer authorization by itself.

Cloud/provider billing may become involved only if an app, agent, chatbot, IDE, terminal runner, backup service, sync service, indexing service, model endpoint, embedding service, OCR/transcription service, code-execution service, or other provider-controlled service receives, processes, uploads, indexes, embeds, stores, or analyzes data from the connected phone or Mac.

PUBLIC_ONLY: confirmed
NO_SECRET_TRANSFER: confirmed
NO_PRIVATE_DEVICE_IDENTIFIERS: confirmed
PHASE_2B_DIRECT_MAC_PHONE_CABLE_PROFILE: active
