# Documenting Economic Security Vulnerabilities

Whereas technical security comes from a lack of bugs in the code, economic security denotes a lack of bugs in the incentives.

Economic security vulnerabilities arise primarily from financial dependencies, which make a protocol's security a function of financial conditions.

This repo is _NOT_ for live vulnerabilities.

## Schema

**Date:** mm/dd/yyyy US Date Standard (not sorry)

**Name:** Default to Twitter (X) name, in case of ambiguity, use existing name for consistency (e.g. if 'Compound Finance' currently in list, use 'Compound Finance' and not 'Compound'), otherwise, use your discretion

**Ecosystem:** 'Ethereum' includes mainnet + rollups including Optimism, Arbitrum, Polygon, etc.

**Protocol Type:** Choose from existing protocol types unless clearly a new category. Avoid subdividing categories, stick to top-level categories (e.g. Lending, not CDP; Stablecoin, not Seignorage Shares).

**Category:** Category of exploit; choose from existing

Price manipulation

Oracle manipulation

**Subcategory** Subcategory of exploit; choose from existing, but subcategories are more flexible

**What happened** A 2-3 sentence description of a description of the incident; simplify - avoid technical terms, function names, etc.
**Value lost by protocol:** Protocol's or users' losses, *not counting a decrease in price of a protocol's governance token*
**Value gained by exploiter** Exploiter's net profit
**Source** Link to a source, or multiple if a single source provides insufficient context
**Vulnerability Level**

Determined by profitability (Y/N) x cost

Low - Unprofitable, permissioned (e.g. upgradable contracts with _no_ exogenous assets)
Medium - Unprofitable, permissionless (e.g. low-cost spam attack)
High - Profitable, permissioned (e.g. governance attack with large capital requirements)
Critical - Profitable, permissionless (e.g. flash loanable price manipulation)


## Definitions

**Price manipulation:** Price is manipulated
**Oracle manipulation:** The oracle, data feed, or data provider to a protocol is manipulated.
