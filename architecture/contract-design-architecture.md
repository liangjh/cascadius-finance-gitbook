---
description: Smart Contract Components in Cascadius - Design
---

# Contract Design Architecture

The basic smart contract components in Cascadius are below.  There will be more complexity in the contracts and connections to indexing infrastructure, but main points are:

* Loan Proxies: Onramp for loan into Cascadius;  contains all indicative, non-PII information on a given loan, and will be made available in the Cascadius loan universe catalog.
* Securitization: represents a full securitization and links to the loan proxy objects that form the collateral base for the securitization, as well as the list of sequential pay classes (in the class of a pass-thru, will link to a single securitization class).
* Securitization Class: represents an an asset that can be held and traded by market participants, and receives proceeds (and incurs losses) from the underlying pool of loans.&#x20;

<figure><img src="../.gitbook/assets/Screen Shot 2022-12-25 at 9.26.25 PM.png" alt=""><figcaption><p>Basic Contract Design Architecture</p></figcaption></figure>

