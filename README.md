# Dallas Crilley

Forward-deployed applied-AI engineer with 10 years turning revenue and operations workflows into production systems. Recent work includes billing automation running for ~19 months, a data backbone spanning six production vendor integrations, and evaluated AI workflows with human approval gates.

**Site:** [dallascrilley.com](https://dallascrilley.com) · **Hiring?** [dallascrilley.com/hire](https://dallascrilley.com/hire) · **Proof ledger:** [dallascrilley.com/proof](https://dallascrilley.com/proof)

## Start with the forward-deployed lifecycle

- [Throughline Connector Kit](https://github.com/dallascrilley/throughline-connector-kit): the sanitized four-method connector contract and sync engine behind six production vendor integrations
- [Shipwright](https://github.com/dallascrilley/shipwright): a tested portfolio implementation of the approved-issue-to-reviewable-PR boundary; live execution is labeled self-reported
- [Winnow](https://github.com/dallascrilley/winnow): lead scoring and routing with a model-evaluation gate, explicit review thresholds, and implementation receipts
- [Vouch](https://github.com/dallascrilley/vouch): human review as an API, with 173 tests and offline end-to-end harnesses using simulated reviewers
- [Holdfast](https://github.com/dallascrilley/holdfast): a production-derived append-only decision ledger and human publish gate rebuilt around a synthetic domain

The full catalog — with sources and caveats for every headline metric — lives on the [proof ledger](https://dallascrilley.com/proof).

**Catalog provenance:** much of this catalog was published to public GitHub in one recent pass while assembling the proof ledger — a repo's publication date is not its development timeline. Where the scaffold-vs-hand-written split matters, the repo carries receipts (e.g. Winnow's [`docs/receipts.md`](https://github.com/dallascrilley/winnow/blob/main/docs/receipts.md)).

## Agent commits

Agents commit under this login; I own the merge gate. The repository's own verification command runs against every change, CI blocks the merge until it passes, and a human makes each irreversible call. Shipwright, Vouch, and Holdfast show those boundaries as working code. Open any repo's history and you can see the split: agent commits carry implementation; my commits set direction, resolve review findings, and cut releases.

## Writing

- [The Four-Method Connector Contract, and Knowing When to Stop](https://dallascrilley.com/writing/throughline-connectors): one connector boundary shared by six vendor integrations
- [When the API Returns 500, Did the Charge Post or Not?](https://dallascrilley.com/writing/meter-idempotent-sync): idempotent billing sync in production
