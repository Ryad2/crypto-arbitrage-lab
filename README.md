# Crypto Arbitrage Lab

A TFA team building low-latency crypto arbitrage research and execution systems.

**Status:** team forming; no live strategy, committed trading capital or performance record is represented by this repository.

## Start here

- Read the [two-page project brief online](https://drive.google.com/file/d/1Is6a29fcmlK_KCePEDWnMb9Hh8WLL_uQ/view?usp=sharing), or use the [repository copy](docs/Crypto_Arbitrage_Lab_TFA_Project_Brief.pdf).
- Check the [open team roles](docs/TEAM.md).
- Review the [first research cycle](docs/RESEARCH_PLAN.md).
- Start from the [initial task board](TASKS.md), then use [Issues](https://github.com/Ryad2/crypto-arbitrage-lab/issues) to claim a task or propose an experiment.
- Contact Ryad in the WhatsApp group **Fund** to join. Send your preferred role, one relevant skill or project, weekly availability and GitHub username.

[TFA project directory](https://docs.google.com/spreadsheets/d/1qoP235Rargd282GHqdJzdVAQDOETdUp7nQacYGlrjZ8/edit?gid=0#gid=0)

## What we are building

We want to establish which price discrepancies survive executable prices, fees, latency and inventory constraints. The first deliverable is one reproducible strategy benchmark, not four simultaneous trading bots.

Research directions include same-chain arbitrage and MEV backrunning, spot/perpetual relative value, prediction-market consistency and cross-chain inventory arbitrage. The team will select one initial route family after reviewing data and access.

The shared pipeline is:

```text
market data -> signal -> cost and risk filters -> replay/simulation
            -> shadow execution -> trade attribution and review
```

Start with Python for research. Add compiled execution components only when measurements justify them. This repository initially contains project documentation and templates, not a working trading engine.

## Working together

1. Agree a small task and its acceptance test in an issue.
2. Use a branch named `research/<topic>` or `feature/<topic>`.
3. Keep a run manifest and separate development data from held-out evaluation.
4. Submit findings or code through a pull request, including negative results.
5. Record decisions in [the decision log](docs/DECISIONS.md).

See [contribution rules](CONTRIBUTING.md) before uploading anything.

## Access and boundaries

This is a private collaboration repository. Ryad will invite confirmed teammates individually; posting its URL does not give others access. There is no public/open-source license in this repository.

Do not upload ArcBook source, employer code, credentials, wallet secrets, personal account exports or restricted market data. Live trading needs a separate explicit decision on access, capital, exposure and loss limits. No live deployment is authorized by joining the project.

The recruitment brief is non-confidential and was shared in Fund on 3 November 2026. Research results and implementation details should stay within the agreed project access until publication is approved.
