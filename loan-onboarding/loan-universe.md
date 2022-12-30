---
description: A Publicly-Searchable On-Chain Loan Marketplace
---

# Loan Universe

Creditors utilize the loan onboarding mechanism in Cascadius to create non-fungible proxies on actual loans.  After a loan is onboarded in this manner, it is immediately available to structuring entities and securitization vehicles on the Cascadius platform. &#x20;

### Loan Catalog / Performance Metrics

Loans are onboarded with a set of detailed but sufficiently granular information about the loan to create a clear picture of credit quality while hiding specific identifying information about the borrower on the loan. &#x20;

Cascadius will provide a series of utilities on the loan market smart contract to search the existing loan universe for active loans by any exposed attribute.  Cascadius will also compile historic performance metrics on the universe, including performance by issuer / vintage / lending program, and groupings by any of the common indicatives.  Making issuer information publicly accessible allows for better price discovery and incentivizes issuers to list loans that remain consistent with the stated intent of their lending programs (whether it is higher performance or higher risk pools).

### Marketplace

Structurers and Issuers would negotiate offline on a fair price for a series of loans, and then transact on the Cascadius loan universe / catalog.  Transactions, again, are conducted with USD-based stablecoins. &#x20;

Post-sale, the structurer (buyer) now owns the proceeds of the loans in the purchased pool.  Note that this is analogous to owning the receivables (and therefore the risk).  The original loan is still serviced by the listing entity, and the proceeds are expected to be transmitted to the structuring entity.&#x20;

At the time of this writing, Cascadius will not be creating a platform for counterparties to trade loan pools.  In the future we can consider building tools to facilitate bids and offers.  &#x20;

Cascadius may also consider creating automated securitizations in the future where loans are selected from the universe on a regular, automated basis.  This would eliminate the structurer from the workflow and make the Cascadius a purely rules-based arbiter between the borrower and investor entities.  We briefly address this in the "Automated Securitization" subsection in "Securitization Methodology".

### Data Storage / Oracles

Loans involve significant amounts information: indicative meta data, credit information, borrower and issuer information and payment histories.  While the smart contracts will store the most basic and up-to-date information on each loan, Cascadius will rely upon compatible decentralized storage and search frameworks.  This feature-rich historical and indicative information will be stored separately from the loan entity and registry on blockchain. &#x20;

We intend to utilize indexing / subgraph protocols such as [TheGraph](https://thegraph.com/en/) to store indicative and transaction histories on listed loans, which can then be utilized as the backing datasource to build oracles to power the loan universe / search capabilities.  We'll expand on this in the service architecture.
