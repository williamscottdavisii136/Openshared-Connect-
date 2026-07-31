# Phase 2C Model Mode Module Enumeration and Revenue Delta Protocol

Date: 2026-07-31
Repository posture: public-safe connector handoff

## Purpose

This record creates a product-by-product protocol for listing modes, models, modules, tool paths, default states, lower-cost alternatives, and revenue-delta tests for AI agents, AI chatbots, coding agents, IDE assistants, terminal agents, open-source agents attached to paid infrastructure, and closed-source AI applications.

## Required matrix fields

Product; category; source status; billing mechanism; available modes; available models; available modules/tool paths; default mode; default model; auto-select status; premium/max/pro/long-context/cloud/agentic/hosted selection status; lower-cost model availability; local/offline/BYOK/MCP/self-hosted/included-plan/zero-incremental-cost route availability; visibility to a lay user; switching difficulty; separately billed modules; task-finality; optional follow-up marking; default-route cost; lower-cost-route cost; quality comparison; time comparison; owner approval/consent; public pricing/documentation source; screenshot/receipt/log/proxy source.

## Initial named products

### Warp / Oz / Warp Agent

Modes/modules to classify: Local Agent, Cloud Agent / Cloud Mode, Agent Mode, Generate, AI Autofill, Active AI, model picker, BYOK/BYOLLM, integrations, tool calls, terminal use.

Cost-control fields: Auto cost-efficiency, model choice, local/self-hosted route, BYOK/BYOLLM, spend limits, add-on credit settings, auto reload settings.

### Visual Studio Code / GitHub Copilot

Modes/modules to classify: Ask, Edit, Agent, Plan, local agents, cloud agents, third-party agents, chat sessions, tool calls, terminal commands, file reads, file edits, search, MCP/custom tools, BYOK.

Cost-control fields: language model picker, auto model selection, organization policy, BYOK provider models, permission controls, reduced context.

### Visual Studio / GitHub Copilot

Modes/modules to classify: Copilot Chat, Agent Mode, Plan Agent, terminal/tool confirmations, code-editing tools, model picker, custom/BYOM models in supported contexts.

Cost-control fields: Plan Agent before Agent Mode, model picker, non-chat premium-model setting, custom/BYOM model where authorized, approval before terminal/tool use.

### OpenAI ChatGPT / Work / Codex

Modes/modules to classify: Chat, Work, Codex, Codex CLI, Codex IDE extension, model picker, credits, Work agent runs, Codex tasks, spreadsheet/presentation/workspace features where available.

Cost-control fields: Instant/Mini where adequate, model picker, Codex `-m` flag/config, local/offline/BYOK/MCP where lawful, stop-at-completion rule, owner approval before credits/overages.

## Revenue-delta test

DEFAULT_ROUTE_COST = credits/tokens/quota/hosted-compute consumed by default mode + default model + default modules.

LOW_COST_ROUTE_COST = credits/tokens/quota/hosted-compute consumed by lower-cost lawful mode + lower-cost model + reduced modules.

REVENUE_DELTA = DEFAULT_ROUTE_COST - LOW_COST_ROUTE_COST.

PERFORMANCE_DELTA = completion quality, time-to-completion, correctness, and user satisfaction difference.

If the low-cost route produces equal or better performance at lower cost, classify the default route as a potential excessive effective-cost, price-gouging indicator, or billing-transparency risk, subject to product-specific evidence.

## Boundary

This record supports consumer-protection R&D, billing transparency, owner consent, cost-control routing, and agency-ready evidence classification. It does not authorize billing circumvention, token/quota/rate-limit evasion, credential capture, session theft, certificate forgery, unauthorized third-party access, public interception, or public service exposure.
