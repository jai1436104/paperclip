# NaadiOS Paperclip Package

This folder is a portable Paperclip company package for **NaadiOS**.

It is meant to be imported into Paperclip as a new company:

```sh
pnpm paperclipai company import ./companies/naadios --target new --yes
```

Recommended follow-up after import:

1. Set the coding agents' adapter working directory to the live product repo at `C:\Users\jai14\Clinic-Agent`.
2. Import or attach your GTM source document `D:\Downloads\Clinic_App_GTM_Strategy.docx` into the NaadiOS wiki or company documents.
3. Keep board approval enabled for new hires and destructive governance changes.
4. Re-enable timer heartbeats only after reviewing each reporting cadence.
5. Feed sanitized operational summaries, not raw patient-sensitive records, into the wiki by default.

The package intentionally separates:

- **active core** for current operating needs
- **vision branch** for future platform expansion
- **portable instructions** in markdown
- **Paperclip-specific runtime fidelity** in `.paperclip.yaml`
