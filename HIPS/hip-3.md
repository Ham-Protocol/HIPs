---
tags: HIPs
---
# HIP 3
```
hip: 3
title: Weights of Yield Farming Pools
author: Eden Au (@edenau), Ivan Martinez (@0xKiwi)
discussions-to: HAM Discord
status: Draft
type: Meta
category Distribution
created: 2020-08-19
requires: 2
replaces: N/A
```

## Simple Summary
Decide the weight of each yield farming pool.

## Abstract
It is crucial to optimize the weight of each yield farming pool to distribute HAM tokens in a fair, inclusive, and diverse manner.

## Motivation
We have seen that having equal distribution among all farming pools would favour those who hold tokens with lower market capitalisation unequally, or end up making the commonly used pools unattractive (Mainly ETH/YFI).

## Rationale
![](https://i.imgur.com/wW1mhv1.png)

#### YAM TVL at Peak (August 13th, 12:30 AM UTC)
**WETH:** 452,474 tokens = $176,463,300
2813 holders in total

**LINK:** 6,644,769 tokens = $106,316,304
1450 holders in total

**YFI:** 13,698 tokens = $73,969,200
1272 holders in total

**LEND:** 138,312,258 tokens = $59,474,270
1694 holders in total

**MKR:** 79,870 tokens = $59,103,800
775 holders in total

**SNX:** 7,402,703 tokens = $39,223,710
1136 holders in total

**COMP:** 165,650 tokens = $33,130,000
1757 holders in total

## Decision
Using the PASTA and YAM pools as reference, we should adjust the pools we have as such:
```
-= Total 1 mil =-
  WETH:    400k
   YFI:    125k
 yyCRV:    150k
   SNX:    100k
  LINK:    100k
  LEND:     100k
  BZRX:     25k
  ```

## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
