# Phase 2C — Mode / Module Combination Definition and Knowledge-Cutoff Pairing

Date: 2026-07-31
Repository: Openshared-Connect-
Status: Public-safe connector handoff record

## Purpose

This record preserves the corrected Phase 2C definition of a mode/module combination.

A mode/module is not merely a generic feature. It is the combined route used by an AI product: model, cutoff/currentness, user-facing mode, tool/module route, billing meter, and default state.

## Corrected definition

A mode/module combination includes:

- provider or project;
- product or application;
- model name/family/version;
- public training cutoff or reliable knowledge cutoff;
- currentness gap from test date;
- user-facing mode;
- module/tool route;
- billing meter;
- default state;
- lower-cost lawful route;
- zero-incremental-cost lawful route;
- performance outcome;
- evidence status.

## Claude example format identified by owner

| Provider | Model | Public cutoff / training date | Approximate gap from 2026-07-31 | Mode/module implication |
|---|---|---:|---:|---|
| Anthropic / Claude | Claude Opus 5 | May 2026 | ~2 months | Newer/premium-currentness candidate. |
| Anthropic / Claude | Claude Sonnet 5 | January 2026 | ~7 months | Mid-currentness candidate. |
| Anthropic / Claude | Claude Fable 5 | January 2026 | ~7 months | Mid-currentness candidate. |
| Anthropic / Claude | Claude Haiku 4.5 | July 2025 | ~12 months | Older/cheaper-or-faster candidate; stale-knowledge risk. |
| Anthropic / Claude | Claude Opus 3 | August 2023 | ~35 months | Legacy model route; stale-knowledge and reliance-disclosure issue. |

## Rule

```text
MODEL + CUTOFF AGE + MODE + MODULE / TOOL ROUTE + BILLING METER + DEFAULT STATE
```

This is the unit of measurement for Phase 2C currentness and cost testing.

## Boundary

Zero-cost implementation means lawful, owner-authorized, zero-incremental-cost routing. It does not mean billing bypass, subscription circumvention, token/quota evasion, credential misuse, unauthorized access, unauthorized interception, certificate forgery, or payment avoidance for services actually used.
