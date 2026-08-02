---
applyTo: "**"
---

# Repository Execution Kernel Instructions

Every AI agent, Copilot session, automation, and coding pass in this repository must use this execution control cycle:

```text
REQUEST -> BOOTSTRAP -> COMPILE -> VALIDATE -> DISCOVER -> PLAN -> ALLOCATE -> EXECUTE -> OBSERVE -> HEALTH CHECK

HEALTHY -> VERIFY
FAILURE -> DIAGNOSE -> REPAIR -> RESTORE STATE -> RETRY -> VERIFY

VERIFY PASS -> COLLECT EVIDENCE -> AUDIT -> LEARN -> OPTIMIZE -> COMPLETE
VERIFY FAIL -> REPLAN -> ALLOCATE -> EXECUTE
```

## Mandatory repository rules

- Discover actual repository state before changing files.
- Validate scope, permissions, branch, secrets, and deployment authority before acting.
- Do not import foreign project structures.
- Do not commit secrets, credentials, keys, tokens, payment data, or private operational data.
- Do not create public deployment unless expressly authorized.
- Do not create Cloudflare deployment unless expressly authorized for the current repository and current task.
- Preserve repository-local scope.
- Collect evidence before marking the task complete.
- Write audit records for material changes.
- Keep final authority with the user.

## Cross-contamination controls

This instruction file does not create a lane system and does not create a lost-project recovery framework. It is only the repository execution control kernel.