# Contribution guide

## Before joining

Message Ryad in Fund with your GitHub username, preferred role and realistic weekly availability. Confirm scope and contribution, ownership and any economic terms before contributing proprietary code. An invitation is not an employment, investment or profit-sharing agreement.

## One task at a time

- Open or claim an issue with a concrete question and acceptance criteria.
- Keep work on a branch and use a pull request for review.
- Document assumptions, data provenance, versions and how to reproduce results.
- Report failed hypotheses and unsuccessful fills; do not silently remove them.
- Do not assign someone else a task or represent them as a teammate without their agreement.

## Data and security

- Never commit secrets, account sessions, private keys, seed phrases or personal account exports, including in screenshots, notebooks or logs.
- Use environment variables or an ignored local secret store for any credentials needed later. Start with read-only access where possible.
- Share only data and code you have permission to use. Do not copy ArcBook or employer material into this repository.
- Store datasets outside Git. Commit a source manifest with permitted access instructions, timestamps, checksums and transformation versions instead.
- Treat external code, notebooks and datasets as untrusted until reviewed.

## Trading boundaries

The initial workflow is replay, simulation and live shadow observation. No funds, trades or paid data subscriptions are authorized by a task assignment.

Transaction-ordering research does not authorize manipulation, sandwiching or misuse of confidential/client order flow. A live pilot requires a separate review and explicit owner approval, including venue eligibility, custody, loss limits and a kill switch.
