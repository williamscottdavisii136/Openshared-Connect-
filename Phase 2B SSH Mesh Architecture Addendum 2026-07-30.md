# Phase 2B SSH Mesh Architecture Addendum

## Purpose

This public-safe Openshared addendum records the SSH mesh layer for the owner-controlled Phase 2B device environment.

No IP addresses, MAC addresses, hostnames, usernames, passwords, SSH private keys, SSH public keys, known_hosts entries, certificates, tokens, phone numbers, serial numbers, IMEIs, private Wi-Fi identifiers, private network diagrams, account secrets, or operational secrets are published here.

## Controlling rule

SSH is authenticated command, file, tunnel, or session access over an IP route.

SSH is not Bluetooth discovery. SSH is not Wi-Fi discovery. SSH is not proof of cloud/provider authorization. SSH requires an IP path, an SSH server on the target where applicable, an SSH client on the origin device, and valid authentication/trust material.

## SSH mesh architecture

```text
SSH CLIENT NODE -> AUTHORIZED IP ROUTE -> SSH SERVER NODE
```

The IP route may be:

```text
Wi-Fi LAN route;
USB tethered IP route where configured and authorized;
Bluetooth PAN route only if specifically configured and authorized;
local Ethernet/adapter route where present;
other owner-authorized local IP route.
```

## What must be in place

```text
1. Origin device has an SSH client.
2. Destination device has an SSH server or SSH-capable service enabled.
3. Destination service listens on an authorized port.
4. IP reachability exists over an authorized local route.
5. Firewall/router/device rules allow the permitted connection.
6. Isolation or security rules do not block the local route.
7. SSH host-key trust is verified.
8. User authentication is authorized.
9. Target account/session is least-privilege for the approved task.
10. Logs and receipts do not publish raw secrets.
11. Each direction is classified separately.
12. Each device class is verified separately.
```

## Full-mesh meaning

Full mesh does not mean unrestricted access. Each approved node-to-node route must be individually classified as:

```text
NO_SSH_ROLE;
SSH_CLIENT_ONLY;
SSH_SERVER_ONLY;
SSH_CLIENT_AND_SERVER;
REACHABLE_AUTHORIZED;
REACHABLE_AUTH_FAILED;
ROUTE_BLOCKED;
HOST_KEY_UNKNOWN;
SERVICE_NOT_RUNNING;
FIREWALL_BLOCKED;
UNVERIFIED.
```

## Billing boundary

Local SSH mesh access is not cloud billing by itself. Local SSH mesh access is not AI-provider billing authorization. Local SSH mesh access is not subscription authorization. Local SSH mesh access is not token/quota authorization.

Cloud/provider billing becomes relevant only if a provider-controlled service receives, processes, meters, stores, or executes the request.

PUBLIC_ONLY: confirmed
NO_SECRET_TRANSFER: confirmed
NO_RAW_SSH_KEYS: confirmed
NO_PRIVATE_NETWORK_IDENTIFIERS: confirmed
PHASE_2B_SSH_MESH_ARCHITECTURE: active
