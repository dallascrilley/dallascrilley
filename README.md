# Dallas Crilley

10 years owning lead-to-cash systems; billing automation in production ~19 months; now shipping evaluated agent systems with human gates. Senior applied-AI and business-systems engineer in Python and TypeScript — evals, tests, and CI, not demos.

**Site:** [dallascrilley.com](https://dallascrilley.com) · **Hiring?** [dallascrilley.com/hire](https://dallascrilley.com/hire) · **Proof ledger:** [dallascrilley.com/proof](https://dallascrilley.com/proof)

## Production extracts

- [Shipwright](https://github.com/dallascrilley/shipwright): an agent that takes an approved GitHub issue and returns a tested, reviewable pull request — it opens the PR only after the target repository's own test command exits zero in a disposable sandbox
- [Vouch](https://github.com/dallascrilley/vouch): human review as an API — agents submit work, real reviewers return a consensus verdict; 173 tests plus offline e2e harnesses
- [Holdfast](https://github.com/dallascrilley/holdfast): append-only decision ledger with a human publish gate, enforced inside Postgres by triggers, a hash chain, and unique indexes; ships adversarial attack tests against its own gate

The full catalog — with sources and caveats for every headline metric — lives on the [proof ledger](https://dallascrilley.com/proof).

## Agent commits

Agents commit under this login; I own the merge gate. The repository's own verification command runs against every change, CI blocks the merge until it passes, and a human makes each irreversible call. The three repos above are that gate as working code: Shipwright won't open a PR until the tests pass, Vouch routes agent output to human reviewers for a consensus verdict, and Holdfast enforces the publish gate inside Postgres. Open any repo's history and you can see the split: agent commits carry the implementation; my commits set direction, resolve review findings, and cut releases.

## Writing

- [The Four-Method Connector Contract, and Knowing When to Stop](https://dallascrilley.com/writing/throughline-connectors): one connector boundary shared by six vendor integrations
- [When the API Returns 500, Did the Charge Post or Not?](https://dallascrilley.com/writing/meter-idempotent-sync): idempotent billing sync in production
