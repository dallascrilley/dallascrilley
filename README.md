# Dallas Crilley

I build the integrations, internal tools, and automation that connect how a business runs. Ten years inside my family's PR firm in Dallas as the only engineer: CRM, billing, six vendor APIs, and lately AI pipelines with a person holding the release button. Python and TypeScript.

**Site:** [dallascrilley.com](https://dallascrilley.com) · **Email:** dallas@dallascrilley.com

## Start here

- [throughline-connector-kit](https://github.com/dallascrilley/throughline-connector-kit): the four-method connector contract and sync engine behind six production vendor integrations, sanitized
- [reconciler](https://github.com/dallascrilley/reconciler): billing discrepancy detection with a required human approval before any invoice changes, on synthetic data; a synthetic rebuild inspired by private Meter billing-audit work
- [vouch](https://github.com/dallascrilley/vouch): human review as an API, with offline end-to-end harnesses that use simulated reviewers
- [shipwright](https://github.com/dallascrilley/shipwright): approved issue to reviewable pull request, with tests on the handoff between agent output and human review
- [holdfast](https://github.com/dallascrilley/holdfast): append-only decision ledger and a human publish gate, rebuilt around a synthetic domain

The production systems these came from (Meter, Throughline, CoHost AI Studio) are private. The site tells each story, including which numbers are self-reported.

Most of this catalog was published in one pass while I assembled the portfolio, so a repo's first commit date is not its development timeline. Where the scaffold-versus-hand-written split matters, the repo says so (see Winnow's [docs/receipts.md](https://github.com/dallascrilley/winnow/blob/main/docs/receipts.md)).

## Agent commits

Agents commit under this login and I own the merge. Each repository's verification command has to pass before I merge, CI runs where it exists, and a person makes every irreversible call. Open any repo's history and the split is visible: agent commits carry implementation, my commits set direction, resolve review findings, and cut releases.

## Writing

- [The Four-Method Connector Contract, and Knowing When to Stop](https://dallascrilley.com/writing/throughline-connectors)
- [When the API Returns 500, Did the Charge Post or Not?](https://dallascrilley.com/writing/meter-idempotent-sync)
