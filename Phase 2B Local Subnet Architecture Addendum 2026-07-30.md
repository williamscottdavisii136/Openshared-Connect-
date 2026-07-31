# Phase 2B Local Subnet Architecture Addendum

## Purpose

This public-safe handoff record preserves the owner-provided local-subnet architecture for Phase 2B device, network, Bluetooth, Wi-Fi, USB, SSH, request, reply, billing, quota, entitlement, and handshake analysis.

## Owner-provided architecture statement

```text
The cell phones, printer, and MacBooks are on a subnet.
```

For public-safe purposes, this means the listed owner-controlled nodes are treated as participating in the same local IP network or locally routed private subnet until exact technical details are separately verified in private.

## Node classes included

```text
cell phones / Samsung smartphones;
Epson WF 2950 printer;
MacBook Air profiles;
MacBook Pro profile;
other owner-controlled subnet nodes only when separately confirmed.
```

## What must be in place for subnet operation

```text
1. A local gateway, router, access point, or LAN segment exists.
2. Each included node has a working network interface.
3. Each included node receives or uses a valid local IP configuration.
4. The nodes share the same subnet, broadcast domain, VLAN, or locally routed private segment.
5. DHCP or static assignment is functioning.
6. Default gateway and DNS behavior are configured where internet access is needed.
7. Local traffic between nodes is not blocked by AP isolation, guest-network isolation, firewall rules, VPN rules, private relay rules, parental controls, or device security settings.
8. Discovery protocols or direct addressing exist where discovery is required.
9. Service-specific listeners exist where services are required.
10. Authentication and authorization exist where SSH, file transfer, printer access, or app control is required.
```

## Layer separation

```text
WI-FI SUBNET:
The subnet is the local IP reachability layer.

BLUETOOTH:
Bluetooth remains peer-to-peer / near-field local connectivity and does not create the subnet by itself.

SSH:
SSH operates over an IP route on the subnet or another authorized IP path; SSH is not created by Bluetooth or Wi-Fi discovery alone.

PRINTER ACCESS:
Printer visibility may use local subnet discovery, direct addressing, printer protocols, or approved Bluetooth profile behavior depending on the actual printer mode.
```

## Boundary

Being on the same subnet may permit discovery or reachability, but it does not by itself prove permission to access files, run commands, print, transfer data, use SSH, share credentials, access certificates, use provider cloud services, or trigger paid services.

Local subnet membership is not AI-provider billing authorization, subscription authorization, token/quota authorization, credential-transfer authorization, certificate-transfer authorization, or proof of cloud entitlement.

PUBLIC_ONLY: confirmed
NO_SECRET_TRANSFER: confirmed
NO_PRIVATE_NETWORK_IDENTIFIERS: confirmed
PHASE_2B_LOCAL_SUBNET_ARCHITECTURE: active
