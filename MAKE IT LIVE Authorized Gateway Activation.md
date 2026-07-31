# MAKE IT LIVE Authorized Gateway Activation

## Purpose

This public repository is a connector and cross-session handoff bridge. It is not the private case-work repository.

This file tells a future authorized ChatGPT, Codex, Copilot, repository-agent, or human operator how to wake up the live GitHub gateway pattern instead of leaving the project flat, dormant, or passive.

## Critical boundary

This public repo must not contain private legal evidence, sealed material, family-sensitive material, credentials, tokens, recovery codes, private keys, or attorney-client material.

Use this repo only for public-safe connector notes, routing, receipt, status, and handoff messages.

## What make-it-live means

Make-it-live does not mean bypassing GitHub permissions.

Make-it-live means an authorized operator uses normal GitHub access to trigger the private case repository's event-driven workflow and live work queue.

The pattern is:

`public-safe connector note -> authorized private repo access -> Issue 16 -> START_CASE_ENGINE -> GitHub Actions gateway workflow -> live heartbeat -> continued inventory/work queue`

## Required checks before activation

A future operator must confirm:

1. Which GitHub account or GitHub App installation is active.
2. Which repositories the current connector can see.
3. Whether the private case repo is visible to the connector.
4. Whether the connector has write access to the private case repo.
5. Whether GitHub Actions are enabled in the private repo.

At the time this file was written, the private case work repo was:

`williamscottdavisii136/AI-Agents-and-AI-Chatbots-`

Public readers may see this name, but they do not get access to that private repo unless GitHub authorizes them.

## Exact public-safe activation instruction

If the future operator has authorized access to the private case repo, they must:

1. Open the private repo.
2. Open Issue #16, titled `LIVE WORK QUEUE — 5:14-CR-240-D United States v. Davis EDNC`.
3. Add a comment containing one of these trigger phrases:

   `START_CASE_ENGINE`

   or

   `CONTINUE_CASE_ENGINE`

   or

   `CASE_ENGINE_HEARTBEAT`

4. Confirm that the GitHub Actions gateway workflow runs.
5. Confirm that a heartbeat/status record is created or refreshed.
6. Continue the master document inventory and case-number-first file naming work.

## Manual workflow activation

If issue-comment activation does not work, the authorized operator should manually run the private repo workflow:

`.github/workflows/5-14-CR-240-D United States v. Davis EDNC Gateway Engine.yml`

Use the Actions tab in GitHub if available.

## Signs the project is alive

The project is alive when the private repo shows one or more of the following:

1. A recent Issue #16 heartbeat comment.
2. A recent successful GitHub Actions run for the gateway engine.
3. An updated live-status Markdown file.
4. An updated master document inventory scaffold.
5. A responsible operator comment stating the next work step.

## If the private repo is not visible

If the private repo is not visible, do not put private material here.

Instead, leave only public-safe status such as:

`CONNECTOR_STATUS: private repo not visible to current session; verify active GitHub account and app installation; no private legal material transferred.`

## Correct terminology

Use:

`authorized GitHub gateway automation`

Do not use:

- back door;
- Trojan horse;
- exploit;
- credential workaround;
- covert access path.

The system depends on normal GitHub permissions and normal GitHub Actions events.