# Dallas Crilley

Forward Deployed / Applied AI Engineer. 10+ years owning the MarTech, RevOps, billing, and operations systems most AI hires have only integrated against — now agent-assisted, shipped with evals, tests, and CI in Python and TypeScript.

Most of my production work lives in private repos. The demos below are public, runnable, and documented — and every one runs a **real server-side backend** on Cloudflare Pages Functions.

**Site:** [dallascrilley.com](https://dallascrilley.com) · **Proof ledger:** [sources and caveats for headline metrics](https://dallascrilley.com/proof/) · **Don't take my word for the backends:** [ping all six live from your browser](https://demos.dallascrilley.com/ops)

## Live demos — six real backends

- [Q2See](https://demos.dallascrilley.com/q2see) — Quote-to-Cash flow inspector; upload a CRM export, the backend flags the broken handoff ([repo](https://github.com/dallascrilley/q2see-demo))
- [Apexlint](https://demos.dallascrilley.com/apexlint) — deterministic linter for agent-written Apex / Flow / n8n, 16 unit-tested rules, no LLM in the loop ([repo](https://github.com/dallascrilley/apexlint-demo))
- [Tracewell](https://demos.dallascrilley.com/tracewell) — flight recorder for AI agents; upload a trace, the backend diagnoses the failure mode ([repo](https://github.com/dallascrilley/tracewell-demo))
- [Inboxward](https://demos.dallascrilley.com/inboxward) — deliverability cockpit with **live SPF / DKIM / DMARC DNS inspection** of any domain ([repo](https://github.com/dallascrilley/inboxward-demo))
- [Forager](https://demos.dallascrilley.com/forager) — Slack-export → confidence-scored Q&A knowledge base via real server-side ingestion ([repo](https://github.com/dallascrilley/forager-demo))
- [Funnelguard](https://demos.dallascrilley.com/funnelguard) — marketing-funnel config linter, 13 deterministic rules ([repo](https://github.com/dallascrilley/funnelguard-demo))

All demo data is synthetic; the engines, tests, and CI are real. Each repo documents its honest real-vs-synthetic boundary.

## Production-shaped public extract

- [Throughline Connector Kit](https://github.com/dallascrilley/throughline-connector-kit) — sanitized four-method connector contract, in-memory sync engine, synthetic CRM example, and tests extracted from the private Throughline production architecture. No client data, credentials, vendor schemas, or private business logic.

## Writing

- [Why I Reduced Integration Code by 40× — and Then Stopped There](https://dallascrilley.com/writing/throughline-connectors) — the four-method connector contract
- [When the API Returns 500, Did the Charge Post or Not?](https://dallascrilley.com/writing/meter-idempotent-sync) — idempotent billing sync in production
