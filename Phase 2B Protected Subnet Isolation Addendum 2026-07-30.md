# Phase 2B Protected Subnet Isolation Addendum

## Purpose

This public-safe Openshared handoff records the owner-provided architecture rule that the Phase 2B home-network/R&D device mesh operates on an owner-controlled subnet isolated from kids, guests, visitors, non-authorized household users, non-authorized smart-device traffic, Bluetooth-only peer traffic, and ordinary internet/Wi-Fi clients unless expressly approved into the subnet.

No SSIDs, Wi-Fi passwords, IP addresses, subnet masks, router addresses, MAC addresses, Bluetooth addresses, hostnames, usernames, SSH keys, tokens, certificates, cookies, sessions, account numbers, phone numbers, serial numbers, IMEIs, or private operational secrets are published.

## Rule

```text
PROTECTED SUBNET: present, owner-stated.
AUTHORIZED SUBNET NODES: owner-controlled cell phones, MacBooks, and printer as previously registered, subject to device-specific verification.
NON-AUTHORIZED / OUTSIDE SUBNET DEVICES: kids, guests, visitors, non-authorized household users, ordinary internet/Wi-Fi clients, non-authorized smart-device traffic, and other devices not approved into the protected subnet.
SMART TV / STREAMING DEVICE TRAFFIC: not assumed to have protected-subnet access unless separately approved and classified.
BLUETOOTH: peer-to-peer / near-field local device connectivity; not subnet access by itself.
INTERNET OVER CABLE ISP / WI-FI: internet route exists separately from protected-subnet authorization.
```

## Classification consequence

Each device or connection class must be tagged as:

```text
protected_subnet_member: yes / no / unknown
internet_access: yes / no / unknown
guest_or_general_network_member: yes / no / unknown
bluetooth_peer_only: yes / no / unknown
smart_device_iot_class: yes / no / unknown
subnet_access_basis: approved owner node / guest-general / denied / unknown
ssh_allowed_to_protected_nodes: yes / no / unknown
printer_allowed_from_protected_nodes: yes / no / unknown
cloud_provider_access: separate evaluation required
ai_provider_billing: separate evaluation required
private_value_published: no
```

## Boundary

Protected-subnet membership is a local-network authorization state. It is not AI-provider billing authorization, subscription authorization, token/quota authorization, credential-transfer authorization, certificate-transfer authorization, or approval to access third-party services.

PUBLIC_ONLY: confirmed
NO_SECRET_TRANSFER: confirmed
NO_PRIVATE_NETWORK_IDENTIFIERS: confirmed
PROTECTED_SUBNET_ISOLATION: active
