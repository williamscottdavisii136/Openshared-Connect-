# Phase 2B Wi-Fi / Xfinity Gateway / Local Discovery / Bluetooth Coexistence Architecture Addendum

## Purpose

This public-safe Openshared handoff records the Wi-Fi architecture needed for all owner-controlled devices to connect through the home-network gateway and see/connect to each other across Wi-Fi, Bluetooth, SSH, USB/direct-link, and local discovery routes.

This record does not publish SSID values, Wi-Fi passwords, router admin credentials, IP addresses, MAC addresses, Bluetooth keys, SSH keys, certificates, tokens, cookies, sessions, phone numbers, IMEI values, serial numbers, private legal materials, or operational secrets.

## Public-safe network description

```text
HOME INTERNET SERVICE CLASS: cable ISP connection, owner-stated
HOME GATEWAY CLASS: Xfinity cable modem / gateway or cable-modem-attached router, owner-stated
PRIVATE WI-FI LABEL: withheld from public record
DEVICE CONNECTIVITY: owner states phones, Macs, printer, smart TV, removable storage when host-mounted, and cable-connected devices can connect through owner-controlled routes
INTERDEVICE TOPOLOGY: owner-controlled local interdevice connectivity / full-mesh intent
```

## Core architecture distinction

Bluetooth and Wi-Fi are separate radio and protocol layers.

```text
WI-FI PATH:
Device Wi-Fi radio -> private Wi-Fi access point / gateway -> local LAN -> optional internet route through cable ISP.

BLUETOOTH PATH:
Device Bluetooth radio -> paired or visible nearby Bluetooth device -> profile-specific service such as pairing, audio, file transfer, PAN/tethering, accessory control, or local device discovery.

SSH PATH:
SSH client -> IP route over Wi-Fi, Ethernet, USB-tethered IP, Bluetooth PAN, or another authorized IP path -> SSH server on target device.
```

Bluetooth does not normally access the Xfinity cable modem or Wi-Fi gateway directly. Bluetooth may coexist with Wi-Fi, pair devices locally, or provide a Bluetooth PAN/tethering path if a host device is configured to bridge or share network access. That bridge/share configuration must be separately verified.

## What must be in place for Wi-Fi to work across all devices

```text
1. Active cable internet service or active local gateway/LAN function.
2. Powered and operational cable modem / gateway / router.
3. Wi-Fi radio enabled on the gateway or attached access point.
4. Private Wi-Fi network broadcast or otherwise joinable by approved devices.
5. Compatible Wi-Fi band and security mode on each device.
6. Correct Wi-Fi credentials or owner-approved join mechanism.
7. DHCP or static IP configuration for each device.
8. DNS and default gateway configuration where internet access is required.
9. Same LAN/subnet or routed LAN segments where device-to-device access is required.
10. AP/client isolation disabled where devices must see each other.
11. Local firewall rules allowing approved discovery and service traffic.
12. Device discovery protocols available where needed, such as mDNS/Bonjour, SSDP/UPnP, printer discovery, app-specific discovery, or direct IP addressing.
13. SSH service enabled on target devices where SSH is intended.
14. SSH client available on initiating devices where SSH is intended.
15. Owner-approved authentication for SSH, file transfer, printer access, media access, app bridge, ADB if enabled, or local device control.
16. No guest-network isolation blocking local-device visibility.
17. No router policy, parental-control rule, VPN profile, private relay, security app, or firewall rule blocking local discovery or interdevice traffic.
18. Sufficient Wi-Fi signal, range, channel availability, and no material radio interference.
```

## Billing boundary

Wi-Fi connectivity, cable modem access, Bluetooth pairing, Bluetooth visibility, SSH reachability, USB direct links, and local discovery are connection states. They are not by themselves AI-provider billing authorization, subscription authorization, token/quota authorization, credential-transfer authorization, certificate-transfer authorization, or third-party cloud-service authorization.

Cloud/provider billing becomes relevant only when an application, agent, chatbot, IDE, terminal runner, sync/backup/indexing service, model endpoint, embedding/vector service, OCR/transcription service, hosted code runner, connector, plugin, marketplace, or other provider-controlled service receives, processes, meters, stores, or executes the request.

PUBLIC_ONLY: confirmed
NO_SECRET_TRANSFER: confirmed
NO_PRIVATE_NETWORK_IDENTIFIER_PUBLICATION: confirmed
PHASE_2B_WIFI_GATEWAY_DISCOVERY_ARCHITECTURE: active
