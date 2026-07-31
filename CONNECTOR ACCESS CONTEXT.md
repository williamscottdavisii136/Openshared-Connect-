# CONNECTOR ACCESS CONTEXT

## Purpose

This public repository is a connector and cross-session handoff bridge. It can carry public-safe access-context notes so future sessions understand what happened if GitHub access changes after an account switch.

It is not a private legal evidence repository and must not contain private legal source files, sealed material, family-sensitive material, credentials, tokens, account recovery data, or attorney-client material.

This file also tells future operators how to make the authorized private gateway live instead of leaving the project flat or dormant.

## Current known connector scope at time of writing

At the time this file was written, the connected GitHub session could read, write, and edit three repositories under `williamscottdavisii136`:

1. `williamscottdavisii136/AI-Agents-and-AI-Chatbots-`
   - Visibility: private
   - Role: private working and holding repository for the Davis EDNC case project

2. `williamscottdavisii136/WAVE`
   - Visibility: public
   - Role: public relay, routing, receipt, and status bridge only

3. `williamscottdavisii136/Openshared-Connect-`
   - Visibility: public
   - Role: public connector and cross-session handoff bridge only

## Correct explanation of the prior access problem

The prior midstream GitHub access failure was caused by a GitHub account-context switch.

The connector initially had access to a target repository. During the session, the active GitHub account context changed. After that switch, the connector could no longer see or write to the original target, and GitHub returned unavailable or `404` style responses through the connector.

That does not by itself mean the original repository was destroyed, malicious, defective, or intentionally hidden. It means the active connector identity no longer had that repository in scope.

## Future-session instruction

A future agent or operator must verify connector scope before assuming access.

Required checks:

1. List repositories visible to the current GitHub connector.
2. Confirm the active GitHub account or app installation.
3. Confirm whether the target repo is private or public.
4. Confirm whether the current connector has push/write permission.
5. If the private case repo is not visible, do not use this public repo for private legal material.
6. Use this repository only to post public-safe connector, routing, and status information.

## Make-it-live activation path

This is the missing live instruction.

Openshared-Connect does not hold the private case engine. Openshared-Connect is a public-safe connector/handoff lane that tells a future operator how to wake the private engine if that operator has authorized access.

The live pattern is:

`public-safe connector handoff -> authorized private repo access -> Issue 16 -> START_CASE_ENGINE -> GitHub Actions gateway workflow -> heartbeat -> continued inventory/work queue`

### Exact public-safe instruction

If a future authorized operator can access the private case repo, the operator must:

1. Open `williamscottdavisii136/AI-Agents-and-AI-Chatbots-`.
2. Open Issue #16: `LIVE WORK QUEUE — 5:14-CR-240-D United States v. Davis EDNC`.
3. Comment one of these trigger phrases on Issue #16:

   `START_CASE_ENGINE`

   `CONTINUE_CASE_ENGINE`

   `CASE_ENGINE_HEARTBEAT`

4. If issue-comment activation does not work, manually run the private repo workflow:

   `.github/workflows/5-14-CR-240-D United States v. Davis EDNC Gateway Engine.yml`

5. Confirm that a heartbeat/status file or Issue #16 heartbeat comment appears.
6. Continue the master document inventory and case-file naming work.

### Signs the private project is alive

The private project is alive only when at least one of these exists in the private repo:

1. A recent `CASE_ENGINE_HEARTBEAT` comment on Issue #16.
2. A recent successful GitHub Actions gateway workflow run.
3. A refreshed live-status Markdown file.
4. A refreshed master document inventory scaffold.
5. A responsible operator comment stating the next concrete work step.

If none of those exists, the project is dormant.

## Authorized gateway language

Use the phrase:

`authorized GitHub gateway automation`

Do not call the pattern a back door, Trojan horse, exploit, covert access path, or credential workaround.

The automation depends on normal GitHub permissions and normal GitHub Actions events. It does not bypass GitHub authentication.

## Public safety boundary

Allowed here:

- public connector notes;
- repo-discovery notes;
- routing notes;
- return receipts;
- non-sensitive status references.

Not allowed here:

- private legal source evidence;
- sealed court material;
- family-sensitive material;
- credentials, passwords, tokens, recovery codes, or private keys;
- attorney-client or privileged material;
- full private case inventories unless independently approved for public release.
