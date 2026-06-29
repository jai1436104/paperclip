# NaadiOS Paperclip Package

This folder is a portable Paperclip company package for **NaadiOS**.

You can import it in two ways.

## Option 1: Import from this local repo clone

```sh
pnpm paperclipai company import ./companies/naadios --target new --include company,agents,projects,tasks,skills --yes
```

## Option 2: Import directly from the GitHub fork branch

```sh
pnpm paperclipai company import jai1436104/paperclip/companies/naadios --ref codex/naadios-company-package --target new --include company,agents,projects,tasks,skills --yes
```

## What This Package Contains

- a NaadiOS company with the active operating core
- a parked future-vision branch
- vendored `paperclip` and `paperclip-create-agent` skills
- starter projects for AGM materials, clinic sales materials, and internal analysis

## Step-By-Step After Import

1. Open the new NaadiOS company in Paperclip.
2. Check that all agents imported and are visible in the org chart.
3. For coding and analysis agents, set the adapter working directory to `C:\Users\jai14\Clinic-Agent`.
4. Keep timer heartbeats disabled at first.
5. Import or upload `D:\Downloads\Clinic_App_GTM_Strategy.docx` into the NaadiOS company documents or wiki.
6. Add your core repo docs from `Clinic-Agent`, especially the README, audit, operator-console plan, and security posture docs.
7. Create or confirm the first three project workstreams:
   AGM materials, clinic sales materials, internal analysis.
8. Review each imported agent before enabling any scheduled heartbeat.
9. Allow only sanitized operational summaries into the wiki first.
10. Keep raw patient-sensitive data out of default agent context.

## Recommended First Activations

Activate these first:

- Wiki Maintainer
- Research Synthesizer
- GTM Lead
- Strategy & Finance Analyst
- Product Engineering Lead
- Operator Console Steward

Then activate:

- Survival Controller
- Infrastructure Capacity Planner
- Test Verification Lead
- Security Compliance Lead
- Sales Partnerships Lead

## Important Guardrails

- keep board approval enabled for new hires and major governance changes
- keep auto-actions limited to low-risk demo acknowledgment, nudges, and scheduling
- do not give default raw patient-record access to analysis agents
- do not let GTM or sales agents promise features that are not in the current product reality

The package intentionally separates the active core, the future-vision branch, portable markdown instructions, and Paperclip-specific runtime fidelity in `.paperclip.yaml`.
