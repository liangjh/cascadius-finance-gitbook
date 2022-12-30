---
description: 'Creating Targeted Risk Profiles: Tranching / Credit Enhancement'
---

# Risk Segmentation

In the prior section we introduced the basic pass-through securitization structure, where all shareholders in the securitization would uniformly incur the same risks and rewards of the underlying loans, in proportion to their ownership of the securitization. &#x20;

### Tranching / Credit Enhancement

Cascadius additionally supports the CDO (collateralized debt obligation) via tranching and credit enhancement in a sequential pay structure, which creates multiple classes on the securitization, each with a asymmetric distribution of risk and return relative to the aggregate pool of underlying loans.  Credit enhancement / tranching creates classes with prioritization on the receipt of proceeds, losses, and principal prepayment.  The classes (an illustrative example below) are tiered:

* Senior classes are prioritized in their receipt of proceeds (principal and interest) from the pool
* If there is unscheduled prepayment of principal from the pool, the senior classes would have priority over the paydown of their principal components, based on their order in the structure.
* Junior (lower) classes incur losses from the pool first.  These classes would be completely dissolved before the senior classes begin to lose principal.   In return for the increased risk, lower classes typically trade at a discount to their total notional value. &#x20;
* Upper classes are deemed more "safe", as they have a higher probability of receiving the full principal of the investment (+ associated interest).&#x20;

<figure><img src="../.gitbook/assets/Screen Shot 2022-12-30 at 8.01.30 AM.png" alt=""><figcaption><p>Loss &#x26; Principal Payment Accrual</p></figcaption></figure>

The initial version of Cascadius will allow for a sequential pay structure: i.e. a simple waterfall-based class structure, like the example highlighted above.  Traditional finance had evolved prior to the financial crisis to support increasingly esoteric structuring variations, but we believe the normal  linear structure would work best to capture a broad variety of risk for all players in the market.

### Esoteric Structures

It's important to be clear about what Cascadius will not support in the near and medium term.   We will not support highly idiosyncratic loan & securitization terms that had become more popular in the immediate years prior to the 2008-2009 global financial crisis.  Esoteric, operationally intensive loan terms evolved to provide flexibility and optionality for larger institutional investors.  A similar parallel evolution had occurred in securitization structures in the race to cater to specific targeted needs of institutional and high net-worth clientele. For a number of reasons, many of these esoteric structures never recovered from their pre-financial-crisis levels, even to the present day.&#x20;

While we believe there can be a niche to support more complexity over time, we believe a more natural and simple onramp would align better with the ethos of transparency and incentivize more mainstream adoption to the Defi ecosystem.
