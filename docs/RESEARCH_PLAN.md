# First research cycle

## Objective

Produce an execution-aware benchmark for one narrow arbitrage route. Decide whether the observed edge survives costs and realistic fills. A useful negative result is a valid outcome.

## Select the first route

Compare a same-chain liquid-token route with a tightly scoped spot/perpetual route. Choose using available data, access constraints, reproducibility, execution complexity and expected inventory needs. Record the decision before building adapters.

Prediction markets and cross-chain routes remain later extensions unless the first data review gives a strong reason to select one instead.

## Proposed six-week cycle

| Stage | Work | Exit evidence |
| --- | --- | --- |
| Week 1 | Agree hypothesis, pair, venues, data and interfaces | Written route decision, access check and timestamped sample |
| Weeks 2-3 | Build replay and try to falsify the hypothesis | Reproducible run, held-out period and cost sensitivity |
| Weeks 4-5 | Observe live signals and simulate execution without funds | Latency and opportunity-decay logs; no assumed guaranteed fills |
| Week 6 | Review and demonstrate the result | Findings, failure cases, reproducibility instructions and go/no-go decision |

This is a proposed sequence, not a confirmed delivery commitment or a live-trading authorization.

## Measurement contract

For each opportunity, record venue/instrument identity, source and local receipt times, quote or order-book state, available depth, intended size and fees. Preserve the data quality and clock-synchronization assumptions.

Do not equate a quoted spread with PnL. For an evaluated route, attribute proceeds less acquisition cost, fees, gas, funding/borrow where relevant, hedging, rebalancing and failure costs. Record any residual inventory and the valuation method; do not count unrealized exposure as a completed arbitrage.

Required outputs include executable-size estimates, fill/partial-fill/revert assumptions, net results over a stated period, latency, capital usage and sensitivity to adverse execution. Keep descriptive estimates separate from realized live results.

## Market-specific checks

- Same-chain and MEV: simulate transaction ordering, gas, reverts and inclusion constraints. Backrunning is not a guarantee of inclusion.
- Spot/perps: include fees, funding at its actual schedule, borrow if applicable, margin, hedge failures and liquidation exposure.
- Prediction markets: compare resolution rules, deadlines, settlement and outcome coverage. Similar titles do not establish equivalent payoffs.
- Cross-chain: use explicit inventory and rebalancing assumptions. Fills on separate chains are not one atomic trade; include delays and interim exposure.

## Reproducibility

Use [the experiment template](EXPERIMENT_TEMPLATE.md). Keep a run manifest with code version, data checksum, configuration, fee schedule and evaluation dates. Separate development and held-out evaluation; include failed or partial executions rather than dropping them.

## Live-pilot gate

Only consider a bounded live pilot after the team reviews evidence, venue/legal eligibility, custody and security. Agree capital, position and daily-loss limits, stop conditions, kill-switch ownership and reconciliation first. No such approval has been given at repository setup.
