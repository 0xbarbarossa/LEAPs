---
leap: 37
title: Deprecate SOL Market
status: Approved 
author: Ksett (@ksett737)
created: 2022-11-14
---

## Simple Summary
Deprecate the SOL market

## Abstract
Deprecate the SOL market 

## Motivation
Given its recent volatility and degradation of liquidity, SOL no longer meets the motivation laid out in LEAP-19 for launching it "SOL is one of the most liquid tokens, attracting large trading volumes across major exchanges, which makes it a suitable candidate for Lyra’s fourth listed asset." as such, the market should be deprecated immediately.

## Specification 
- Allow remaining SOL positions to close only 
- Add no additional expiries or strikes in the SOL markets 
- Allow delta hedging to continue through the last expiration, Nov 25th 
- Block any new deposits from entering the SOL MMV
- LP rewards and  trading rewards should continue as planned through the Nov 25th expiry and then cease

### Rationale
The unknown future state of liquidity and the binary nature of the potential price movement in the Solana market makes it an inappropriate asset for the AMM. Listing additional options on SOL would create undue risk for LPs. SOL should be delisted as an asset and re-evaluated once market conditions normalize.

### Configurable Values
SOL market parameters will be determined by CCs.
short collateral rewards = 0
trading rewards = 0

## Test Cases
N/A

## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
