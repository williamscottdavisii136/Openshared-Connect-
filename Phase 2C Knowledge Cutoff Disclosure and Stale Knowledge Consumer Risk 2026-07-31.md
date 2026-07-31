# Phase 2C Knowledge Cutoff Disclosure and Stale Knowledge Consumer Risk

Date: 2026-07-31

## Public-safe connector note

This record adds a Phase 2C public-safe lane for AI knowledge cutoff, stale training data, currentness disclosure, and consumer reliance.

## Core point

Many users may not understand that an AI chatbot, AI agent, coding agent, terminal agent, or app-builder product may be operating from a model snapshot rather than current knowledge. Currentness depends on the specific model, version, mode, and whether live search, retrieval, file context, connector access, or other current-data routes are active.

## Public-source example

Official Anthropic / Claude documentation identifies model-specific knowledge or training cutoffs and warns that models may lack accurate information after their cutoffs.

Sources:

- https://support.claude.com/en/articles/8114494-how-up-to-date-is-claude-s-training-data
- https://platform.claude.com/docs/en/about-claude/models/overview

## Risk labels

- KNOWLEDGE_CUTOFF_DISCLOSURE_RISK
- STALE_KNOWLEDGE_RISK
- OUTDATED_TRAINING_DATA_RISK
- CURRENTNESS_MISREPRESENTATION_RISK
- FALSE_CURRENT_AUTHORITY_RISK
- PROFESSIONAL_RELIANCE_RISK
- CONSUMER_NONCONSENT_RISK
- BILLING_FOR_STALE_OUTPUT_RISK
- LIVE_SEARCH_ABSENCE_RISK
- RETRIEVAL_NOT_ACTIVE_RISK
- MODEL_SNAPSHOT_DISCLOSURE_RISK

## Required product test

For each product: capture model, model ID/version, mode, module/tool route, training cutoff, reliable knowledge cutoff, live search status, retrieval status, connector/file status, disclosure state, billing unit, and lower-cost/current-data alternative.

## Boundary

This lane does not assert that every provider hides knowledge cutoffs or that every model is a year behind. It requires product-specific proof and supports lawful consumer-protection R&D, billing transparency, and informed consent.
