# Phase 2B Bluetooth Visibility Pairing and Full Mesh Architecture Addendum

## Purpose

This public-safe Openshared addendum describes what must be in place for Bluetooth functionality to work across the owner-controlled Phase 2B device environment.

The key distinction is that Bluetooth visibility, Bluetooth pairing, Bluetooth profile access, Wi-Fi/IP connectivity, SSH connectivity, and full-mesh interdevice communication are separate layers.

A device may see another device over Bluetooth without being authorized to transfer files, run commands, share internet, access app data, access storage, use SSH, or reach any cloud provider.

PUBLIC_ONLY: confirmed
NO_SECRET_TRANSFER: confirmed
NO_PRIVATE_DEVICE_IDENTIFIERS: confirmed
NO_RAW_BLUETOOTH_KEYS: confirmed
NO_RAW_SSH_KEYS: confirmed
NO_RAW_CERTIFICATE_VALUES: confirmed

## Architecture distinction

```text
BLUETOOTH VISIBILITY:
A device is advertising, discoverable, or responding to scan/inquiry.

BLUETOOTH PAIRING / BONDING:
The devices have accepted a pairing/trust relationship and stored non-public link/security material inside their operating-system Bluetooth stores.

BLUETOOTH PROFILE ACCESS:
The devices support a matching service/profile such as audio, keyboard/mouse, file transfer, printer discovery, tethering/PAN, serial/RFCOMM, BLE GATT, or device-specific control.

WI-FI / IP CONNECTIVITY:
The devices are on the owner-controlled network route and can resolve/reach each other by IP, local hostname, mDNS/Bonjour, SSDP, or another local discovery method.

SSH CONNECTIVITY:
A host is running an SSH server, the client can reach the host over an IP route, and authorized host/user authentication succeeds.

FULL-MESH INTERDEVICE CONNECTIVITY:
The owner-controlled devices can communicate through approved Wi-Fi/IP, Bluetooth, USB/USB-C cable, SSH, local storage, or other authorized local routes. Full mesh does not mean every Bluetooth device can maintain every Bluetooth profile to every other device at the same time.
```

## What must be in place

```text
1. Bluetooth-capable hardware on each device.
2. Working OS Bluetooth driver/stack.
3. Bluetooth radio powered on.
4. Device discoverability or advertising enabled where needed.
5. Nearby physical range and tolerable radio interference.
6. Required app/system permissions enabled.
7. Pairing/bonding when required.
8. Matching Bluetooth profiles/services on both sides.
9. User approval for trust prompts or pairing prompts where required.
10. Device-specific restrictions satisfied.
11. Stored pairing/bonding material not deleted, expired, reset, or rejected.
12. Requested service/profile enabled after pairing.
```

## Billing consequence

Bluetooth visibility, pairing, Bluetooth profile access, Wi-Fi discovery, SSH reachability, and USB visibility are local connection states. They do not by themselves establish AI-provider billing authorization, cloud entitlement, subscription entitlement, token/quota authorization, provider account authorization, certificate-transfer authority, credential-transfer authority, or paid resource approval.

Cloud/provider billing becomes relevant only if a provider-controlled service receives, processes, stores, meters, or executes the request.

PHASE_2B_BLUETOOTH_ARCHITECTURE: active
