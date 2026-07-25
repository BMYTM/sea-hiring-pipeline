# HONO · SEA Hiring Pipeline Portal

A lightweight, self-contained hiring pipeline tracker for HONO.ai's Southeast Asia GTM & delivery recruiting. Open roles and candidate pipelines organised **by country** — Philippines, Indonesia, Malaysia (with country heads) and Singapore, Thailand, Vietnam (led directly by the SEA Business Head).

**Live app:** open `index.html` — no build, no backend, no dependencies.

## Features

- **KPI dashboard** — open roles, seats to fill, candidates, in-interview, offers out, hired (live).
- **Country tabs** — each shows its country head and open roles.
- **Role cards** — function, level, seat count, status (Open / Urgent / On-hold), hiring manager, target close date, and a live pipeline funnel.
- **Candidate kanban** — five stages (Sourced → Screening → Interview → Offer → Hired). **Drag cards between stages** to update.
- **Embedded job descriptions** — Thailand roles include a "View JD" panel; full JDs live in [`/roles`](./roles).
- **Add / edit / delete** roles and candidates, including a LinkedIn URL per candidate.
- **Persistence** — auto-saves to the browser (localStorage). **Export** to a JSON file to back up or move machines; **Import** to restore. **Reset sample** restores the built-in demo data.

## Open roles — Thailand (hiring now)

| Role | Function | Level | JD |
|---|---|---|---|
| Payroll Functional Consultant | Implementation | Mid–Senior | [JD](./roles/thailand-payroll-functional-consultant.md) |
| L1 Support Specialist | Support | Junior–Mid | [JD](./roles/thailand-l1-support.md) |
| Operations Lead | Operations | Senior | [JD](./roles/thailand-operations-lead.md) |
| Talent Acquisition Specialist | People / TA | Mid | [JD](./roles/thailand-talent-acquisition.md) |

## Run it

Just open `index.html` in any modern browser. To host it for the team, drop the repo on **GitHub Pages** (Settings → Pages → deploy from `main` / root) and share the URL.

## Data model

All state lives in one JSON object (`countries → roles → candidates`). Export produces exactly this shape, so it's easy to script against or migrate into an ATS later.

## Notes

The seeded candidates in Philippines, Indonesia, Malaysia, Singapore and Vietnam are **illustrative sample data** to show the tool working. Thailand's four roles are the current live openings and start with empty pipelines, ready for sourcing.

---
Built for Boonchoo Malhotra · HONO SEA.
