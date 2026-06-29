# NaadiOS Company Package Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Create a portable Paperclip company package for NaadiOS with the approved org tree, agent instructions, and Paperclip sidecar config so it can be imported into a Paperclip instance.

**Architecture:** Keep the deliverable markdown-first and import-friendly. Put the company package under `companies/naadios/`, define every agent as an `AGENTS.md`, and keep adapter/runtime/reporting fidelity in `.paperclip.yaml`. Vendor the core Paperclip runtime skills into the package so imports do not depend on external skill resolution.

**Tech Stack:** Markdown package files, YAML sidecar config, Paperclip company portability format.

---

### Task 1: Create the package root

**Files:**
- Create: `companies/naadios/COMPANY.md`
- Create: `companies/naadios/README.md`
- Create: `companies/naadios/.paperclip.yaml`

- [ ] Define the NaadiOS company root, import notes, and Paperclip sidecar.
- [ ] Encode the approved org tree, adapter defaults, governance defaults, and intended cadence.

### Task 2: Create the active-core agents

**Files:**
- Create: `companies/naadios/agents/ceo-naadios/AGENTS.md`
- Create: `companies/naadios/agents/survival-controller/AGENTS.md`
- Create: `companies/naadios/agents/operator-chief/AGENTS.md`
- Create: `companies/naadios/agents/operator-console-steward/AGENTS.md`
- Create: `companies/naadios/agents/product-engineering-lead/AGENTS.md`
- Create: `companies/naadios/agents/test-verification-lead/AGENTS.md`
- Create: `companies/naadios/agents/infrastructure-capacity-planner/AGENTS.md`
- Create: `companies/naadios/agents/security-compliance-lead/AGENTS.md`
- Create: `companies/naadios/agents/gtm-lead/AGENTS.md`
- Create: `companies/naadios/agents/sales-partnerships-lead/AGENTS.md`
- Create: `companies/naadios/agents/strategy-finance-analyst/AGENTS.md`
- Create: `companies/naadios/agents/wiki-maintainer/AGENTS.md`
- Create: `companies/naadios/agents/research-synthesizer/AGENTS.md`

- [ ] Write each active agent with a concrete charter, inputs, outputs, cadence, escalation rules, and data-sensitivity boundaries.

### Task 3: Create the vision agents

**Files:**
- Create: `companies/naadios/agents/future-platform-strategist/AGENTS.md`
- Create: `companies/naadios/agents/care-network-referral-strategist/AGENTS.md`
- Create: `companies/naadios/agents/patient-intelligence-strategist/AGENTS.md`

- [ ] Add the future-vision branch as on-demand agents with no scheduled heartbeat by default.

### Task 4: Vendor the core Paperclip skills

**Files:**
- Create: `companies/naadios/skills/paperclip/**`
- Create: `companies/naadios/skills/paperclip-create-agent/**`

- [ ] Copy the required Paperclip skills into the package so imported agents can resolve `paperclip` and `paperclip-create-agent` locally.

### Task 5: Verify structure and document usage

**Files:**
- Verify: `companies/naadios/**`

- [ ] Check the package tree and spot-check the key files against the Paperclip portability docs.
- [ ] Document the exact import command for local use.
