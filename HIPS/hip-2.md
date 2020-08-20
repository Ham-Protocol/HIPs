---
tags: HIPs
---
# HIP 2
```
hip: 2
title: Yield Farming Pools for Initial HAM Distribution
author: Eden Au (@edenau), Ivan Martinez (@0xKiwi), Cucurbit (@PiperCucu)
discussions-to: HAM Discord
status: Draft
type: Meta
category Distribution
created: 2020-08-15
requires: N/A
replaces: N/A
```

## Simple Summary
Decide which tokens can farm HAM.

## Abstract
Farming for HAM is the most essential component of HAMs distribution, so it is important to properly decide which tokens should be allowed for farming, which rationale as to why, and which tokens should not be allowed with rationale as to why not. 
For decentralization, a chain is as strong as its weakest link. Meaning if there is a method of earning HAM where certain individuals outweigh others, it could be detrimental to the protocol and its ditribution. This could be seen with LEND and COMP, where existing holders of said tokens earned an extreme amount more compared to ETH or MKR.

## Motivation

The more tokens we allow, the more careful we have to be with each of their relative HAM returns, but the less we allow, the more we may possibly restrict the distribution of HAM.

Restricting the amount of tokens could also be more powerful as we could make the lesser tokens individually more rewarding, and allow for specific demographics (such as strictly ETH holders) to join the effort. This could be powerful in ensuring HAM holders are passionate, share similar interests, and are driven towards benefiting the protocol.

## Rationale

![AMPL token distribution](https://i.imgur.com/Dx3FyCr.png)

![DeFi token distribution](https://i.imgur.com/MD60qrs.png)
<!--source: https://twitter.com/coinbureau/status/1294059672283029505/photo/1-->

Looking at the tokens used by YAM, there are some questionable decisions. Judging by the above charts of distribution, we believe AMPL_ETH_UNI_LP, COMP and LEND are too centrally distributed to be considered for stakedropping.

## Personal study of distribution at peak of YAM craze:
### Distribution 24 hours from launch, before the yCRV pool.
```
Distribution for LEND out of total 99868796 tokens
The top 1 holder has 8.0105% of pool (8000000 tokens)
The top 5 holders have 27.9686% of pool (27931879 tokens)
The top 10 holders have 41.1999% of pool (41145842 tokens)
The top 25 holders have 56.3775% of pool (56303547 tokens)
The top 50 holders have 67.7775% of pool (67688563 tokens)
The top 100 holders have 78.3717% of pool (78268842 tokens)
The top 250 holders have 90.1015% of pool (89983309 tokens)
1407 holders in total (99868796 tokens)
```
```
Distribution for LINK out of total 5659490 tokens
The top 1 holder has 7.6728% of pool (434241 tokens)
The top 5 holders have 26.7154% of pool (1511955 tokens)
The top 10 holders have 44.2812% of pool (2506091 tokens)
The top 25 holders have 66.1407% of pool (3743224 tokens)
The top 50 holders have 79.6561% of pool (4508131 tokens)
The top 100 holders have 88.9245% of pool (5032674 tokens)
The top 250 holders have 96.7266% of pool (5474231 tokens)
1106 holders in total (5659490 tokens)
```
```
Distribution for MKR out of total 54664 tokens
The top 1 holder has 17.6478% of pool (9647 tokens)
The top 5 holders have 36.7902% of pool (20111 tokens)
The top 10 holders have 52.3763% of pool (28631 tokens)
The top 25 holders have 71.5059% of pool (39088 tokens)
The top 50 holders have 82.4235% of pool (45056 tokens)
The top 100 holders have 90.7178% of pool (49590 tokens)
The top 250 holders have 97.9475% of pool (53542 tokens)
659 holders in total (54664 tokens)
```
```
Distribution for SNX out of total 6446789 tokens
The top 1 holder has 11.7699% of pool (758783 tokens)
The top 5 holders have 30.3209% of pool (1954727 tokens)
The top 10 holders have 41.6966% of pool (2688090 tokens)
The top 25 holders have 56.9953% of pool (3674369 tokens)
The top 50 holders have 69.9874% of pool (4511941 tokens)
The top 100 holders have 82.9647% of pool (5348556 tokens)
The top 250 holders have 94.7563% of pool (6108736 tokens)
890 holders in total (6446789 tokens)
```
```
Distribution for WETH out of total 402815 tokens
The top 1 holder has 7.4476% of pool (30000 tokens)
The top 5 holders have 27.3465% of pool (110156 tokens)
The top 10 holders have 39.0951% of pool (157481 tokens)
The top 25 holders have 55.3949% of pool (223139 tokens)
The top 50 holders have 66.7512% of pool (268884 tokens)
The top 100 holders have 79.1348% of pool (318767 tokens)
The top 250 holders have 91.9271% of pool (370296 tokens)
2086 holders in total (402815 tokens)
```
```
Distribution for YFI out of total 12568 tokens
The top 1 holder has 5.9755% of pool (751 tokens)
The top 5 holders have 23.1143% of pool (2905 tokens)
The top 10 holders have 35.0175% of pool (4401 tokens)
The top 25 holders have 52.4268% of pool (6589 tokens)
The top 50 holders have 68.5471% of pool (8615 tokens)
The top 100 holders have 82.4157% of pool (10358 tokens)
The top 250 holders have 94.7167% of pool (11904 tokens)
1127 holders in total (12568 tokens)
```
```
Distribution for COMP out of total 97588 tokens
The top 1 holder has 5.6595% of pool (5523 tokens)
The top 5 holders have 17.4468% of pool (17026 tokens)
The top 10 holders have 27.1878% of pool (26532 tokens)
The top 25 holders have 42.0820% of pool (41067 tokens)
The top 50 holders have 54.0394% of pool (52736 tokens)
The top 100 holders have 68.2317% of pool (66586 tokens)
The top 250 holders have 85.3906% of pool (83331 tokens)
1357 holders in total (97588 tokens)
```
### Distribution at peak YAM, right before the second rebase.
```
Distribution for LEND out of total 138312258 tokens
The top 1 holder has 20.8224% of pool (28799976 tokens)
The top 5 holders have 38.5009% of pool (53251523 tokens)
The top 10 holders have 49.1171% of pool (67935005 tokens)
The top 25 holders have 64.8403% of pool (89682091 tokens)
The top 50 holders have 74.2479% of pool (102693880 tokens)
The top 100 holders have 83.2809% of pool (115187719 tokens)
The top 250 holders have 92.4656% of pool (127891228 tokens)
1694 holders in total (138312258 tokens)
```
```
Distribution for LINK out of total 6644769 tokens
The top 1 holder has 7.5637% of pool (502590 tokens)
The top 5 holders have 25.2612% of pool (1678551 tokens)
The top 10 holders have 41.4549% of pool (2754580 tokens)
The top 25 holders have 62.0422% of pool (4122564 tokens)
The top 50 holders have 78.3024% of pool (5203014 tokens)
The top 100 holders have 88.1644% of pool (5858318 tokens)
The top 250 holders have 96.3115% of pool (6399677 tokens)
1450 holders in total (6644769 tokens)
```
```
Distribution for MKR out of total 79870 tokens
The top 1 holder has 42.0083% of pool (33552 tokens)
The top 5 holders have 55.2348% of pool (44116 tokens)
The top 10 holders have 66.8724% of pool (53411 tokens)
The top 25 holders have 81.6752% of pool (65234 tokens)
The top 50 holders have 89.0647% of pool (71136 tokens)
The top 100 holders have 94.6388% of pool (75588 tokens)
The top 250 holders have 99.0146% of pool (79083 tokens)
775 holders in total (79870 tokens)
```
```
Distribution for SNX out of total 7402703 tokens
The top 1 holder has 10.2501% of pool (758783 tokens)
The top 5 holders have 28.5211% of pool (2111331 tokens)
The top 10 holders have 39.0068% of pool (2887556 tokens)
The top 25 holders have 54.4945% of pool (4034067 tokens)
The top 50 holders have 67.6026% of pool (5004422 tokens)
The top 100 holders have 80.9460% of pool (5992194 tokens)
The top 250 holders have 93.6405% of pool (6931925 tokens)
1136 holders in total (7402703 tokens)

```
```
Distribution for WETH out of total 452474 tokens
The top 1 holder has 11.1131% of pool (50284 tokens)
The top 5 holders have 32.3387% of pool (146324 tokens)
The top 10 holders have 42.7386% of pool (193381 tokens)
The top 25 holders have 57.5996% of pool (260623 tokens)
The top 50 holders have 68.7025% of pool (310861 tokens)
The top 100 holders have 79.5641% of pool (360007 tokens)
The top 250 holders have 91.8539% of pool (415615 tokens)
2813 holders in total (452474 tokens)
```
```
Distribution for YFI out of total 13698 tokens
The top 1 holder has 5.4826% of pool (751 tokens)
The top 5 holders have 21.5725% of pool (2955 tokens)
The top 10 holders have 32.5887% of pool (4464 tokens)
The top 25 holders have 50.8906% of pool (6971 tokens)
The top 50 holders have 67.3894% of pool (9231 tokens)
The top 100 holders have 81.6835% of pool (11189 tokens)
The top 250 holders have 94.5978% of pool (12958 tokens)
1272 holders in total (13698 tokens)
```
```
Distribution for COMP out of total 165650 tokens
The top 1 holder has 42.8765% of pool (71025 tokens)
The top 5 holders have 51.8750% of pool (85931 tokens)
The top 10 holders have 58.0085% of pool (96091 tokens)
The top 25 holders have 66.0809% of pool (109463 tokens)
The top 50 holders have 73.4778% of pool (121716 tokens)
The top 100 holders have 81.8400% of pool (135568 tokens)
The top 250 holders have 92.0350% of pool (152456 tokens)
1757 holders in total (165650 tokens)
```
```
Distribution for AMPL_ETH_UNI_LP out of total 3662694656195230964 tokens
The top 1 holder has 4.1116% of pool (150593544726913024 tokens)
The top 5 holders have 16.1161% of pool (590285204019824196 tokens)
The top 10 holders have 26.5411% of pool (972119479446798329 tokens)
The top 25 holders have 44.4767% of pool (1629046967348413060 tokens)
The top 50 holders have 59.2748% of pool (2171054123619152903 tokens)
The top 100 holders have 73.9463% of pool (2708428656236273116 tokens)
The top 250 holders have 90.0567% of pool (3298500814921746462 tokens)
1293 holders in total (3662694656195230964 tokens)
```
```
Distribution for YAM_YCRV_UNI_LP out of total 1825047 tokens
The top 1 holder has 3.5261% of pool (64353 tokens)
The top 5 holders have 11.8150% of pool (215630 tokens)
The top 10 holders have 19.6645% of pool (358886 tokens)
The top 25 holders have 36.6161% of pool (668261 tokens)
The top 50 holders have 53.3428% of pool (973532 tokens)
The top 100 holders have 70.6525% of pool (1289442 tokens)
The top 250 holders have 88.5469% of pool (1616023 tokens)
1041 holders in total (1825047 tokens)
```

![](https://i.imgur.com/9cfshLT.png)


## Decision
**WETH:** Yes, community support and fairly split

**LINK:** Yes, community support and fairly split

**SNX:** Yes, community support and fairly split

**YFI:** Yes, community support and fairly split

**yyCRV:** Yes, community support and fairly split

**LEND:** Yes, community support and fiarly split 

**BZRX:** Yes, small cap (will be weighted) but community support

**COMP:** No, not fair and community rejected

**MKR:** No, not fair and community rejected

**AMPL_ETH_UNI_LP:** No, community rejected


## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).


