---
description: Main Architectural Components, Services & Models
---

# Service Architecture

### High-Level Architecture

The main high-level system components for Cascadius are below.  The decentralized nature of the EVM blockchain environment and existing indexing services greatly simplifies the overall infrastructural components of Cascadius. &#x20;

* EVM-compatible smart contracts: smart contracts for (a) Loans, and (b) Securitizations serves as the heart of the Cascadius system: verifiable and decentralized registries for proxied loan assets and securitized pools.
* Smart contracts control the distribution of proceeds from the pool to holders of the securitization and enforce the distribution rules of the waterfall.
* Historic information / payments & transactions are stored outside of the smart contract.  The precise indexing technology / platform is still under consideration, but will store historic information for all collateral on Cascadius.
* Smart contracts emit events when state changes or is modified on either the loan or pool / securitization objects; events will be consumed by the indexing nodes, our primary store of historic information.
* As indexed historical data will be made public, users can query the index nodes for collateral information, build their own reporting, or utilize pre-built reporting from Cascadius.  Reporting may be hosted centrally by Cascadius for faster access.
* The pricing engine is a long-term goal given the compute-heavy nature of securitized products models.  As a result, the pricing service may be a separate, centrally-hosted component of Cascadius.  Details TBD.

<figure><img src="../.gitbook/assets/Screen Shot 2022-12-25 at 9.27.28 PM.png" alt=""><figcaption><p>Main System Components</p></figcaption></figure>

These are the main components.  We will update with integration guides & developer's guides closer to launch.
