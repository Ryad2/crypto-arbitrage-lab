# Experiment record

Copy this template for a specific experiment and link it from its issue.

## Question and hypothesis

State the proposed edge and what observation would disprove it. Identify the exact instruments, venue or chain, route and size being evaluated.

## Data and run manifest

- Owner and issue:
- Code commit and environment:
- Data source and permitted access:
- Capture period, time zone and timestamp conventions:
- Data location and checksum:
- Missing/stale/out-of-order data handling:
- Configuration and fee/funding schedule:
- Development and held-out evaluation periods:

## Execution model

Explain executable pricing/depth, latency, order submission or inclusion assumptions, partial fills and failed legs. State inventory, hedge and rebalancing assumptions. List included costs and any unresolved material cost separately.

## Acceptance and falsification tests

Define the success criteria before reviewing the held-out result. Include a baseline and at least one adverse latency, cost or fill scenario.

## Results

Distinguish measured observations, model assumptions, simulated results and realized trades. Include negative cases, residual exposure, capital usage and uncertainty. Link reproducible commands and artifacts without uploading restricted data or secrets.

## Decision

Continue, change the hypothesis or stop. Explain why, and name the next test if any. A research conclusion is not authorization to deploy funds.
