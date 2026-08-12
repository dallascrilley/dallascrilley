# Dallas Crilley

Applied AI and forward deployed engineer. Ten-plus years owning the MarTech, RevOps, billing, and operations systems most AI hires have only integrated against. The newer layer on top is agent systems shipped with evals, tests, and CI, in Python and TypeScript.

Most of my production work lives in private repos. The demos below are public, runnable, and documented, and every one runs a **real server-side backend** on Cloudflare Pages Functions.

**Site:** [dallascrilley.com](https://dallascrilley.com) · **Proof ledger:** [sources and caveats for headline metrics](https://dallascrilley.com/proof/) · **Don't take my word for the backends:** [ping six of the seven live from your browser](https://demos.dallascrilley.com/ops). The seventh, the RevOps factory, makes real model calls, so you run it from its own demo page instead.

## Live demos: seven real backends

- [RevOps Software Factory](https://dallascrilley.com/demos/revops-factory): multi-agent review of a synthetic revenue batch; a coordinator dispatches dedup, attribution, and stage-logic agents and returns one verdict with a live token-cost ledger ([repo](https://github.com/dallascrilley/revops-factory-demo))
- [Q2See](https://demos.dallascrilley.com/q2see): Quote-to-Cash flow inspector; upload a CRM export and the backend flags the broken handoff ([repo](https://github.com/dallascrilley/q2see-demo))
- [Apexlint](https://demos.dallascrilley.com/apexlint): deterministic linter for agent-written Apex / Flow / n8n, 16 unit-tested rules, no LLM in the loop ([repo](https://github.com/dallascrilley/apexlint-demo))
- [Tracewell](https://demos.dallascrilley.com/tracewell): flight recorder for AI agents; upload a trace and the backend diagnoses the failure mode ([repo](https://github.com/dallascrilley/tracewell-demo))
- [Inboxward](https://demos.dallascrilley.com/inboxward): deliverability cockpit with **live SPF / DKIM / DMARC DNS inspection** of any domain ([repo](https://github.com/dallascrilley/inboxward-demo))
- [Forager](https://demos.dallascrilley.com/forager): turns a Slack export into a confidence-scored Q&A knowledge base via real server-side ingestion ([repo](https://github.com/dallascrilley/forager-demo))
- [Funnelguard](https://demos.dallascrilley.com/funnelguard): marketing-funnel config linter, 13 deterministic rules ([repo](https://github.com/dallascrilley/funnelguard-demo))

All demo data is synthetic; the engines, tests, and CI are real. Each repo documents exactly what is real and what is synthetic.

## Production-shaped public extract

- [Throughline Connector Kit](https://github.com/dallascrilley/throughline-connector-kit): sanitized four-method connector contract, in-memory sync engine, synthetic CRM example, and tests extracted from the private Throughline production architecture. No client data, credentials, vendor schemas, or private business logic.

## Released tools: Waves 1–4

- **Agent and delivery systems:** [Broadside](https://github.com/dallascrilley/broadside), [Shipwright](https://github.com/dallascrilley/shipwright), [Yardmaster](https://github.com/dallascrilley/yardmaster), [Quorum](https://github.com/dallascrilley/quorum), [Muster](https://github.com/dallascrilley/muster), [Onward](https://github.com/dallascrilley/onward)
- **Developer tools:** [Polycast](https://github.com/dallascrilley/polycast), [XAir CLI](https://github.com/dallascrilley/xair-cli), [Vaultkeep](https://github.com/dallascrilley/vaultkeep), [Trifold](https://github.com/dallascrilley/trifold), [RepoMan](https://github.com/dallascrilley/repoman), [Placard](https://github.com/dallascrilley/placard)
- **Evaluation and inspection:** [Gradewell](https://github.com/dallascrilley/gradewell), [Dowser](https://github.com/dallascrilley/dowser), [Winnow](https://github.com/dallascrilley/winnow), [Marrow](https://github.com/dallascrilley/marrow), [Reconciler](https://github.com/dallascrilley/reconciler)
- **Presentation and packaging:** [Showwright](https://github.com/dallascrilley/showwright), [Deckhand](https://github.com/dallascrilley/deckhand), [Outfitter](https://github.com/dallascrilley/outfitter)

- **Wave 4 production extracts:** [Cinderwell](https://github.com/dallascrilley/cinderwell) runs disposable cloud dev servers under self-destructing leases; [Tenantwell](https://github.com/dallascrilley/tenantwell) proves Postgres row-level tenant isolation; [Holdfast](https://github.com/dallascrilley/holdfast) keeps an append-only decision ledger behind human publication approval; [Landfall](https://github.com/dallascrilley/landfall) migrates WordPress sites to Astro and verifies URL parity.

## Writing

- [The Four-Method Connector Contract, and Knowing When to Stop](https://dallascrilley.com/writing/throughline-connectors): one connector boundary shared by six vendor integrations
- [When the API Returns 500, Did the Charge Post or Not?](https://dallascrilley.com/writing/meter-idempotent-sync): idempotent billing sync in production
- [The Gate Has to Stand Without the LLM](https://dallascrilley.com/writing/cohost-eval-gate): deterministic metrics block, LLM evals advise, a human owns the irreversible call

## The commit graph below this README

The graph shows more than 100,000 commits in the past year. Agents wrote most of them. I run coding agents in parallel worktrees through the workday, they commit under my login, and each of those commits lands on the graph.

I author the layer that decides whether agent work survives. The repository's own verification command runs against every change, CI blocks the merge until it passes, and a human makes each irreversible call. Three of the released repos are that layer as working code: [Shipwright](https://github.com/dallascrilley/shipwright) opens a pull request only after the target repository's test command exits zero in a disposable sandbox, [Quorum](https://github.com/dallascrilley/quorum) sends agent output to human reviewers who return a consensus verdict, and [Reconciler](https://github.com/dallascrilley/reconciler) blocks invoice changes until a person approves the flagged discrepancy.

Open any repo's history and you can see the split. Agent commits carry the implementation. My commits set direction, resolve review findings, and cut releases.
