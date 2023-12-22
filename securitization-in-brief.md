---
description: Who are the main players in a securitization?  How does securitization work?
---

# Securitization In Brief

To provide some context for Cascadius, we illustrate the mechanics of securitized markets and how borrowers and investors are connected.&#x20;

### Borrowers and Investors

Borrowers (retail or institutional) require capital to finance asset purchases (i.e. via a loan).  The most prominent asset that borrowers purchase is for residential property, but this can also apply to any asset. \*\*

Banks typically play the role of the primary lender to retail borrowers and underwrite loans.  The bank decides whether the borrower is extended credit.  However, banks have limited capital and risk requirements, and so reach a point at which they are capital constrained, but also by the mismatch in their assets and liability maturities.&#x20;

On the other end are investors who seek yield and diversification, and are willing to assume risk to achieve higher yield.&#x20;

<figure><img src=".gitbook/assets/Screen Shot 2022-12-29 at 11.01.00 PM.png" alt=""><figcaption><p>Looks like an opportunity to connect borrowers and investors</p></figcaption></figure>

### Enter Securitization

Securitization combines loans into special purpose vehicles (i.e. SPVs) which distribute proceeds from the loan pool.  In traditional finance, broker-dealers (i.e. investment banks) play the role of structurer and market maker.  Cascadius will also rely upon structurers to do the same, but provide the basic tooling to create simple pass-through as well as tranched structures on the blockchain.

Securitization in TradFi makes the process of connecting borrowers and lenders scalable by bundling pools of smaller loans together at a volume that would allow for the participation of institutional players.  In the case of the simple pass-through structure, all investors receive the same aggregate proceeds and accumulate the same aggregate losses from the loans in the pool.&#x20;

<figure><img src=".gitbook/assets/Screen Shot 2022-12-29 at 11.10.04 PM.png" alt=""><figcaption><p>An SPV allows the two sides to connect.</p></figcaption></figure>

Collateralized Debt Obligations define prioritized classes with asymmetric distribution of proceeds, losses, and recoveries.  Tranching creates a spectrum of risk / reward profiles, which target investors with different risk appetites.  The process is illustrated below:

<figure><img src=".gitbook/assets/Screen Shot 2022-12-29 at 11.26.14 PM.png" alt=""><figcaption><p>Tranching caters to a diverse range of investors</p></figcaption></figure>

Traditional securitized finance had evolved significantly in the last several decades: from mortgage pass throughs issued by the GSEs (FNMA / FHLMC) to CMOs & CDOs (collateralized mortgage and debt obligations) with more sophisticated structures involving credit enhancement / over-collateralization, interest and principal-only tranches, and pari-passu structures.  Additionally, securitizations evolved to support additional loan types, including commercial MBS, auto, student loans, and more.  The era leading up to the global financial crisis saw increasingly esoteric structures including synthetic CDOs and CDS.  Rampant speculation and financial engineering through synthetics were largely responsible for amplifying the impact of the financial crisis in 2008-2009.  We'll link to more literature and research on these topics in the appendix.&#x20;

### Cascadius Finance

Cascadius provides the scaffolding to facilitate securitizations on EVM-compatible blockchains, creating a verifiable and transparent marketplace for the transmission of risk and capital financing.   Our goal is to start with the essentials to achieve securitization, and expand to an increasing set of use cases.  The base set needed in Cascadius include the following:

* The proxy tokenization of loans and lending products
* A framework to create and manage securitized vehicles on the blockchain
* A marketplace for investors to transact on securitizations&#x20;
* Flow of proceeds and losses between counterparties
* Reporting and basic analytics and access to historical performance information

_\*\* Note that the underwriting and due diligence process can differ widely depending on the type of asset being financed and the target market / borrower.  Cascadius Finance does not address the origination / underwriting of loans._
