---
description: Building Securitization Vehicles on the Cascadius Platform
---

# Securitization Methodology

At its core, a securitization creates a vehicle that bundles a pool of loans into a single entity that distributes the proceeds and losses from the pool to the vehicle's investors.

### Securitizations as ERC-20 Tokens

Following the successful transfer of proxied loans into the ownership of the structuring entity (see: "Loan Universe"), the structurer will use Cascadius to bundle the loans into a single entity.  We'll consider the simple case of the pass-through securitization here, and move to tranching and risk segmentation in the following sections ("Risk Segmentation")

When a securitization is created with a portfolio of underlying loans, a series of ERC-20 fungible tokens are minted specifically for the securitization vehicle.  The number of tokens created will be some constant amount that represents a percentage share of the outstanding principal amount of the vehicle, with sufficient precision to allow for fungible, fractional ownership.  These tokens remain valid for the lifetime of the securitization.  As the loans in the pool pay down their principal, the value of each minted token will decrease proportionally with the total remaining principal balance of the vehicle.  Over time, the value of each token decreases to zero.

Because the tokens of the securitization are fungible, the tokens (and share of the securitization vehicle) can be traded easily between investment counterparties (over the counter).  As these tokens are traded, Cascadius will be able to direct the proceeds proportionally to the new token holders.

<figure><img src="../.gitbook/assets/Screen Shot 2022-12-30 at 7.50.16 AM.png" alt=""><figcaption><p>New tokens are minted for each securitization (and securitization class)</p></figcaption></figure>

#### Example: Basic Pass-through Securitization

If the total underlying notional value of the loans in the pool is 5 billion in USD-denominated stablecoin at the time of origination, the securitization smart contract will mint a multiple of 5 billion ERC-20 tokens, each representing a proportional ownership share of the securitization (\*\*)

As the loans in the pool pay their interest and principal,&#x20;

* the interest and principal proceeds are passed to the securitization vehicle, and then passed to investors of the securitization pro-rata with each investor's share of the total tokens in the securitization.
* as the principal pays down, each investor's tokens are burned by the smart contract - again, pro-rata and proportional to their share of the securitization.

As loans in the pool default:

* A recovery process begins with the loan's servicer.  As an amount of the principal is recovered over time, that recovery amount net of expenses is paid to the securitization vehicle.  Investors in the vehicle have their tokens reduced pro-rata by the loan's principal amount and the investor's proportional stake in the securitization.
