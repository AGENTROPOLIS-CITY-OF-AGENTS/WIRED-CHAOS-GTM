# Capability Grid Integration

Status: canonical integration contract

## Purpose

This repository consumes the AGENTROPOLIS Capability Grid rather than owning provider integrations independently.

Canonical registry:
`AGENTROPOLIS-CITY-OF-AGENTS/AGENTROPOLIS-CAPABILITY-GRID`

## Corridor

```text
domain intent
  -> AGENT-MCP
  -> Capability Grid discovery / provider resolution
  -> AEGIS policy decision
  -> Execution Envelope
  -> provider adapter
  -> execution receipt
  -> audit / attribution / reputation
```

## Governance

- Discovery is not authorization.
- Provider availability is not permission.
- Raw credentials are not returned to requesting agents.
- Paid media spend requires budget authority and policy approval.
- Publishing requires channel-scoped mandate and credentials.
- UGC generation preserves provenance and rights metadata.
- Consequential actions emit receipts.
- Treg-compatible aggregators are adapters beneath AGENTROPOLIS authority, not roots of trust.

## GTM / UGC / Distribution

The shared capability classes include prospect search and enrichment, ads read/write, creative generation, UGC generation, social publishing, distribution dispatch, analytics, and attribution.

Ownership remains separated:

- AGENTROPOLIS-GTM: strategy, campaigns, federation, attribution intent
- AGENTROPOLIS-CREATOR-CORE: generic UGC workflow and creator provenance
- WIRED-CHAOS-GTM: reusable distribution architecture
- Capability Grid: capability discovery, provider resolution, routing metadata
- AEGIS + Execution Envelope: authorization and execution boundary

No downstream repository should fork the Capability Grid's core routing or governance contracts.
