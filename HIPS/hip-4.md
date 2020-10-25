---
tags: HIPs
---
# HIP 4
```
hip: 4
title: Method of Treasury Accrual
discussions-to: HAM Discord
status: Accepted
type: Meta
category Distribution
created: 2020-08-20
requires: N/A
replaces: N/A
```

## Simple Summary
Decide the method for accruing value in the HAM piggy bank (treasury).

## Abstract
HAM serves as limitless voter rights to the treasury and protocol, so it is important to build up a treasury that can back up the value of HAM, and allow HAM to serve as rights over.
This HIP will look into possible ways of accruing value into the treasury, and their pros and cons.

## Options For Bootstrapping The Treasury

### Rebase
**Pros:**
- Scales well with price, encourages constant funding during positive rebasing
- Automatic, no holder interaction needed.
- Sell pressure is predictable at set times

**Cons:**
- Negative rebasing is a very dangerous territory
- Integration with other smart contracts is risky/discouraged
- Gimmicky, possibly losing interest

**Note:** Negative rebasing could be disabled entirely or only at launch, and only enabled by a vote.

### Farmer Tax
Every harvest performed on the staking contracts, a percent (maybe 1%) is sent to a contract sells on Uniswap, and sends the purchased token to the treasury.

**Pros:**
- Elegant solution, no modification to token needed
- Scales well with interest in HAM

**Cons:**
- Runs dry after farming is over
- Sell pressure is not predicatable, and X% of entire supply.

### Transfer Tax
Every transfer of the token includes a second transfer of a small % (maybe 0.5%) that is sent into a contract that sells the token on uniswap, and sends the purchased token to the treasury.
A transfer tax would also be a tax on harvest, since a harvest is a token transaction.

**Pros:**
- Sustainable, continues providing funding long after farming
- Can also act as a farmer tax

**Cons:**
- Modification directly into the token
- Tokens with built in fees could be problematic for smart contracts
- Discourages trading on DEXes

### Treasury Minting Tax
We replace the rebases with a dynamic minter that prints based off of the price or price movement, to sell onto uniswap into the treasury.

**Pros:**
- No more rebases, reduced complexity
- Since the treasury is the only thing minting, could possibly derive more value than rebasing

**Cons:**
- No more price "stability"
- We're literally the fed
- Dilutive to voters

## Decision
We will stick with rebases, as they offer a good narrative (stable-value) and offer a sustainable method of treasury accrual.

## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
