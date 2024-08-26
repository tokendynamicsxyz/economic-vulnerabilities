# Documenting Economic Security Vulnerabilities

Whereas technical security comes from a lack of bugs in the code, economic security denotes a lack of bugs in the incentives.

Economic security vulnerabilities arise primarily from financial dependencies, which make a protocol's security a function of financial conditions.

This repo is _NOT_ for live vulnerabilities.

## Examples

The protocol design process can be broken up into four stages:
1. Validation - The gathering of _**business requirements**_, resulting in a _**product spec**_ is validated by an the gathering of resources toward a protocol's development.
2. Design - Business requirements are translated into a _**design spec**_ that describe at a high level _how the protocol works_; evaluated with a design audit/economic security assessment.
3. Architecture - Modules are arranged such that the protocol is technically secure and gas efficient, resulting in _pseudocode_, evaluated as part of a technical audit.
4. Code - Functions are chosen, pseudocode is translated into actual _code_, evaluated in a technical audit.

Economic vulnerabilities arise from mistakes in the design. While protocol development is not always so straightforward, these vulnerabilities arise from the _non-technical considerations_ in protocol development.

Because of this, they are concerned with a set of disciplines that lie outside of the typical developer's expertise (e.g. economics, mechanism design, financial engineering). Economic vulnerabilities are marked by mistakes of this nature.

## Schema

**Date:** mm/dd/yyyy US Date Standard (not sorry)

**Name:** Default to Twitter (X) name, in case of ambiguity, use existing name for consistency (e.g. if 'Compound Finance' currently in list, use 'Compound Finance' and not 'Compound'), otherwise, use your discretion

**Ecosystem:** 'Ethereum' includes mainnet + rollups including Optimism, Arbitrum, Polygon, etc.

**Protocol Type:** Choose from existing protocol types unless clearly a new category. Avoid subdividing categories, stick to top-level categories (e.g. Lending, not CDP; Stablecoin, not Seignorage Shares).

**Category:** Category of exploit; choose from existing

- Price manipulation
- Oracle manipulation

**Subcategory** Subcategory of exploit; choose from existing, but subcategories are more flexible

**What happened** A 2-3 sentence description of a description of the incident; simplify - avoid technical terms, function names, etc.

**Value lost by protocol:** Protocol's or users' losses, *not counting a decrease in price of a protocol's governance token*

**Value gained by exploiter** Exploiter's net profit

**Source** Link to a source, or multiple if a single source provides insufficient context

**Vulnerability Level**

Determined by profitability (Y/N) x barriers to execution

- **Low:** Unprofitable, permissioned (e.g. upgradable contracts with _no_ exogenous assets)
- **Medium:** Unprofitable, permissionless (e.g. low-cost spam attack)
- **High:** Profitable, permissioned (e.g. governance attack with large capital requirements)
- **Critical:** - Profitable, permissionless (e.g. flash loanable price manipulation)

## Definitions

**Price manipulation:** Price is manipulated.

**Oracle manipulation:** The oracle, data feed, or data provider to a protocol is manipulated.

_P.S. "Flash loan" is not a category of economic exploit. A flash loan is a method for exploiting vulnerabilities. You may be looking for **Price manipulation** category, or **Critical** level vulnerability._
