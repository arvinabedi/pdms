# PDMS: packaging design workflow

**Order, assign, iterate, approve, deliver.** The packaging team's order and approval system, built in Persian, with reports on how long the work really takes.

| | |
|---|---|
| **Role** | Sole builder |
| **When** | September 2026. The first working version took two days. |
| **Stack** | Node + Express 5, Zod, MySQL with versioned migrations, React 19 + Vite; right-to-left Persian UI |
| **Size** | ~22,000 lines · 29 server test files · 14 commits |
| **Status** | Runs on the company server under [Tool Hub](https://github.com/arvinabedi/tool-hub) at `/pdms`, with accounts and roles kept in step with Tool Hub |

> The source is private company code at Ronix Tools. I'm glad to walk through it in an interview. → [Portfolio](https://arvinabedi.github.io)

## The flow

```
Commercial team files an order
      ↓
Packaging lead assigns a designer
      ↓
Designer uploads draft versions ── feedback ──┐
      ↓                                        │
Approval  ←───────────────────────────────────┘
      ↓
Delivery + reporting on real turnaround
```

## Things I cared about

- **Every version is kept.** The history of a design shows exactly what was asked for and what changed.
- **One identity across the company's tools.** People don't get a second password: accounts and PDMS roles are managed from Tool Hub.
- **Installable by IT without me.** A step-by-step Windows install (including a path that needs no Administrator rights), a runbook, demo data, and release notes for every version.
- **Persian first.** The whole interface is right-to-left Persian, because that's the language the people using it work in.

---

[Portfolio](https://arvinabedi.github.io) · [All case studies](https://github.com/arvinabedi)
