---
tags: HIPs
---
# HIP 5
```
hip: 5
title: Funding Public Goods through Farmer Tax
author: Ivan Martinez (@0xKiwi), Eden Au (@edenau)
discussions-to: HAM Discord
status: Accepted
type: Meta
category Distribution
created: 2020-08-21
requires: N/A
replaces: N/A
```

## Simple Summary
Decide on where and how much fund from farming should go towards funding public goods such as Gitcoin Grants, and other various dev-focused projects.

## Abstract
While HAM's goal is to build a treasury, it is also important that we give back to the community in a way that does not take funds from the treasury.

### Farmer Tax Towards Gitcoin
Every harvest performed on the staking contracts, a percent (maybe 1%) is sent to a contract sells on Uniswap, and sends the purchased token to the treasury.

**Pros:**
- Elegant solution, no modification to token needed
- Scales well with interest in HAM
- Sells at a rate over time, rather than a full allocation.

**Cons:**
- Runs dry after farming is over
- Sell pressure is not predictable, and X% of entire supply.

## Decision
We have reached the decision to implement a 1% farmer tax on harvest that would be contributed towards Gitcoin directly.

## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
