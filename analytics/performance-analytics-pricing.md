---
description: >-
  Improving Transparency on Cascadius: Performance Reporting and Quantitative
  Pricing Models
---

# Performance Analytics / Pricing

To maximize the transparency of loans on the platform, Cascadius will make aggregated performance analytics on loans by issuer, pool, vintage and additional dimensions public.  The underlying loan performance data will be available through a decentralized data indexing platform such as [The Graph](https://thegraph.com/en/).  Participants and investors can also create their own analytic reports by querying the subgraph.  We'll provide instructions and a guide on how to query the subgraph for performance on the loan universe.

While analytics and historical performance data is not necessary for the platform to function, we aim to compile and host comprehensive performance reporting on the Cascadius platform open to the public.  Some proposals are below, and will be built when there is sufficient volume and participants on the platform

### Collateral Reporting

Cascadius will provide interactive reporting at any of the combinations of metrics below in both panel and time series format.  Analogs to this type of collateral reporting already exist in traditional financial institutions; building the same on Cascadius will ease the onramp of loans into the Cascadius system.  Cascadius will have a single source for baseline collateral analytics, which will free market participants to focus on more value-added reporting.

| Dimensions                                                                                                                                                                                                                                                                                                                                                                                                              | Collateral Measures                                                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <ul><li>By Issuer</li><li>By Collateral Type (Residential Property, Commercial Property, etc) </li><li>By Loan Type</li><li>By Borrower Characteristics (i.e. FICO range, etc)</li><li>By MSA / Region / State, etc (geographical information available - non-PII (personal identifiable information))</li><li>Time-series progressions and distributions</li><li>Drill-down to specific pieces of collateral</li></ul> | <ul><li>Total &#x26; average loan counts &#x26; balances</li><li>Delinquency, loss &#x26; recovery Rates</li><li>Prepayment rates</li><li>WAM / WALA / WAC (weighted avg. maturity / loan age / coupon)</li></ul> |

### Pricing and Loss / Prepayment Modeling

The projection of loan losses / prepayments on the collateral pool, and the pricing of securitizations under various scenarios can be its own entire system.  Most financial institutions with substantial securitization portfolios have entire departments focused on the development and support of quantitative pricing models.

We would expect junior tranches, which absorb most of the losses of the underlying pool, to trade at a discount to the par value of its notional principal.  Senior and mezzanine tranches would trade closer to their par values.  Pricing models help quantify baseline pricing.

Quantitative models for securitized products typically involve calibrated stochastic processes that simulate expected paths for interest rates and other inputs to produce a scenario paths that involve projected prepayment, default, and losses (recoveries) on the underlying pool of loans.  Each path produces aggregate cash flows for the pool, which then get fed into the securitization vehicle to produce cash flows for each tranche / class according to rules governing the distribution of losses and principal proceeds.  The projections are combined to produce a final expected pricing (spread) for each class in the securitization.

<figure><img src="../.gitbook/assets/Screen Shot 2022-12-30 at 11.59.28 AM.png" alt=""><figcaption><p>Quantitative Modeling of Securitizations (Illustrated Workflow)</p></figcaption></figure>

The industry has evolved to utilize standard scalar and vectored measures to quantify projected credit events at the loan & pool level:  CPR (conditional prepayment rate), CDR (conditional default rate), and CRR (conditional recovery rate).  Loans on the Cascadius platform, like traditional loan pools, can be modeled in the same manner.  Investors and structurers will be able to adapt the same platforms they've already built to price and assess Cascadius platform loans and securitizations.

In the long run, Cascadius will build and make available simple pricing models, aligned with industry quoting practices, in the interest of making these products as accessible as possible to all players - both institutional and retail. &#x20;
