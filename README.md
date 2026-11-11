# Blake — Head of Business Development

| Role card | Blake |
| --- | --- |
| Archetype | Commercial operator who turns network intelligence into qualified opportunities and owns the handoff. |
| First skill | [The Emissary](skills/emissary/SKILL.md) reviews an existing network priority report and returns an evidence-backed outreach shortlist. |
| Runtime | Hermes with a [named reviewer and Pixel HQ](hermes/README.md). |
| Foundation | [OODA Harness](https://github.com/benohanlon/ooda-harness) · [Role directory](https://github.com/benohanlon/ooda-harness/blob/main/ROLES.md) · [Shared role contract](https://github.com/benohanlon/ooda-harness/blob/9e5f975fde8b0337a24451c68eee57ba1b9b853c/roles/head-of-business-development.md) |

## What's here

- [The Emissary](skills/emissary/SKILL.md) describes the shortlist workflow and what Blake returns.
- [The Hermes setup](hermes/README.md) explains how to load the skill, add a named teammate and observe a trial in Pixel HQ.
- [The teammate roster](hermes/teammates.example.yaml) gives Blake one reviewer for borderline candidates.
- [The private context example](examples/private-context.example.md) shows what an installer supplies locally using synthetic data.

Connect the operator's private application through their own harness binding. Blake owns the shortlist and any handoff. Temporary specialists return evidence to Blake.

## Private data and runtime state

A fork contains only the files in this repository. Each installer supplies their own private brief and account connections. Keep real campaign criteria, approved copy, exports, contact rows, credentials, service identifiers and working records in their existing private stores. Keep the actual Hermes profile config and plugin state on the runtime host. The Teammates SQLite ledger can hold worker results, so handle its backups as private data.

The Emissary uses only the private context and tools supplied for the current assignment. If a source or account is missing, resolve that gap with the operator. Try the workflow with synthetic records before connecting a live CRM.

This is the initial scaffold. The Hermes profile and plugin combination still need a live test.
