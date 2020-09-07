---
tags: HIPs
---
# HIP 6
```
hip: 6
title: Distribution and Liquidity Provision Structure
author: Ivan Martinez (@0xKiwi), Eden Au (@edenau), Gabriel Saunders (@Ponjinge1)
discussions-to: HAM Discord
status: Accepted
type: Meta
category Distribution
created: 2020-08-24
requires: 3
replaces: N/A
```

## Simple Summary
It is important to structure seeding distribution and liquidity rewards in a way that incentives farmers staying active, and encourages price action. This is a HIP to help outline possible schedules and methods for liquidity provision.

## Abstract
There are limitless ways to reward liquidity and multiple projects have tested various methods. Some were extremely simple like YAM (seed farming followed by a 50/50 pool 24 hours later), while some were much more complex like YFV, having multiple waves and several different types of pools.

## Distinctions Between Types of Pools
### 50/50 Liquidity Pools
* Most common.
* Requires buying the asset for most people, especially if on Uniswap.
* Largest impermanent loss out of all.

### 98/2 Liquidity Pools
* One of the safest liquidity pool setting for risk-averse farmers.
* Not on Uniswap.
* Balancer allows single asset entry.
* Encourages mild price action. Any entries into the pool pump the price of the 2% asset. Good for sustaining price.
* Almost like holding the 98% of the primary asset.

### Seed Stake-farming
* The least risky.
* Allows for initial audience capture and distribution.
* Highest TVL.

## Waves
The concept of waves helps farmers slowly adapt and move into different positions of different risk and keep them constantly engaged in the community. Separating pools into waves is important for building structure with the farmers and providing ample time for the treasury to accumulate and use cases to form.

### Wave 1 (Seed farming):
Should be as risk free as possible, initial seed farming through various coins. Should be the lowest in rewards compared to all waves. Mainly for driving interest.
Rebase could be enabled at this point.

### Wave 2 (Mild risk liquidity mining):
Introduce the milder risk liquidity pools with a 98/2 ratio on Balancer with higher rewards to keep farmers engaged. Should increase rewards compared to wave 1.
Rebase could be enabled at this point.


### Wave 3 (Riskier liquidity mining):
Followed by the riskiest AMM pool with a 50/50 ratio. This pool encourages the most trading and price action, so it is crucial to ensure liquidity providers are strongly incentivized.

## Examples
YFV pool schedule:
![](https://i.imgur.com/XJtI2Lf.png)
YFV supply allocated per pool:
![](https://i.imgur.com/0l94WbE.png)

Issues with this:
* Too many pools, all spread out to a very long duration. Too much competition.
* Liquidity needs to be bootstrapped.

However, YFV community had voted to burn the supply dedicated for the 50/50 pool thinking less supply would be beneficial, but this results in less upwards price action for the coin.

## Decision
![](https://i.imgur.com/H0f044V.png)

![](https://i.imgur.com/QlPe2k7.png)


## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
