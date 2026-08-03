# Openshared-Connect-

A bidirectional **account bridge** that connects two GitHub accounts —  
**[williamscottdavisii136](https://github.com/williamscottdavisii136)** and **[Billydeeii136](https://github.com/Billydeeii136)** —  
enabling cross-account collaboration, communication, and shared repository access through dual tunnels.

---

## How the Bridge Works

```
williamscottdavisii136                    Billydeeii136
        │                                       │
        │  ──── Tunnel A (→) ────────────────►  │
        │                                       │
        │  ◄──── Tunnel B (←) ────────────────  │
        │                                       │
        └────────── bridge-config.yml ──────────┘
```

| Tunnel | Direction | Purpose |
|--------|-----------|---------|
| **Tunnel A** | `williamscottdavisii136` → `Billydeeii136` | Push updates, dispatch events |
| **Tunnel B** | `Billydeeii136` → `williamscottdavisii136` | Receive events, pull updates |

---

## Repository Structure

| File | Purpose |
|------|---------|
| `bridge-config.yml` | Bridge and tunnel configuration — lists both accounts, tunnel directions, and shared repositories |
| `.github/workflows/bridge.yml` | GitHub Actions workflow — validates the config, sends cross-account events (Tunnel A), and receives incoming events (Tunnel B) |

---

## Setup Instructions

### 1. Fork / mirror this repository under the secondary account

In the **Billydeeii136** account, create (or fork) a repository named `Openshared-Connect-` and add the same `bridge.yml` workflow.

### 2. Create a Personal Access Token (PAT)

1. Go to **Settings → Developer settings → Personal access tokens** under `williamscottdavisii136`.
2. Generate a **classic** PAT with `repo` scope.
3. Add `Billydeeii136` as a collaborator on that account's repository so the token can dispatch events.

### 3. Add the secret to both repositories

In each repository go to **Settings → Secrets and variables → Actions → New repository secret**:

| Secret name | Value |
|-------------|-------|
| `BRIDGE_TOKEN` | The PAT generated above |

### 4. Trigger the bridge

- Push a commit to `main` in either repository.
- The **Tunnel A** job automatically notifies the other account.
- The **Tunnel B** job wakes up and acknowledges the event.
- Both accounts can now monitor each other's activity through the Actions tab.

---

## Customising the Bridge

Edit `bridge-config.yml` to:
- Add more repositories under each account.
- Change tunnel behaviour (e.g. enable `sync_pull_requests`).
- Add additional accounts to the bridge.

---

## Connected Accounts

- 🟢 **williamscottdavisii136** — primary
- 🟢 **Billydeeii136** — secondary
