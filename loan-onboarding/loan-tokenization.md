---
description: Onboarding Loan Assets to the Cascadius Platform
---

# Loan Tokenization

Loans listed on Cascadius are assumed to have already been underwritten by an issuer.  Note that the Cascadius platform will not underwrite or service loans, as loan underwriting can be an entire system / protocol of its own, per product type.

Listing on Cascadius requires transmitting the main loan terms, some basic indicative information about the borrower, any payment history on the loan, as well as issuer information.

Cascadius Finance \* **creates a proxy** by which any loan (real / traditional, or on Defi) with a regular repayment schedule can be exposed on the blockchain by a creditor or servicing entity.   Note that the original loan (as well as the servicing or management of any collateral) is not handled by Cascadius. &#x20;

### Loans as ERC-721 / ERC-1155 Tokens

Cascadius will effectively mint an ERC-721 / ERC-1155 compatible token for each loan exposed on the platform, which will each serve as a proxy for the loan.

By listing a loan on the Cascadius platform, a creditor / servicer allows the loan's proceeds to be purchased by a structuring entity, and subsequently packaged into a securitization.

Loans are onboarded with a set of detailed but sufficiently granular information about the loan to create a clear picture of credit quality while hiding specific identifying information about the borrower on the loan.  This includes basic loan terms (duration / payment schedule), loan type and issuer, vintage and issuance details, and some meta-information about the collateral for the loan.  As the information will be searchable publicly, we do not require or allow specific identifying information about the borrower or collateral type to list.

Each loan, through its ERC-721 proxy, is indivisible and cannot be partitioned further.  The indivisibility of the loan allows the entire loan entity to be transferred / purchased.  The loan is therefore unique; it cannot be subdivided, and is non-fungible.  \*\*

The Cascadius platform will support a growing series of loan types at various payment frequencies, with the initial supported loan types for fixed-rate and fixed-term.  While each loan is a unique minted non-fungible token (NFT), all tokens will have common properties that will allow counterparties to interact on the marketplace.

The smart contracts facilitating loan proxy creation assigns and validates ownership of loans and facilitates the flow of funds through the lifecycle of the loan and its subsequent securitization. &#x20;

### Transacting on Cascadius

All transactions within Cascadius are done with USD-backed stablecoins (USDC, Tether).  We utilize stablecoins in order to minimize the volatility associated with other native tokens.  Utilizing stablecoins as the transaction medium for loan proceeds and recoveries allows for an easier onramp for off-chain assets.  We expect most of our initial off-chain loans to be denominated in USD or other fiat currencies.  Loans in other fiat currencies can assume the foreign exchange risk inherent in conversion to USD.   Cascadius may support other fiat currencies in the future as well.

### Lifecycle Management

#### Delinquencies & Recoveries

As Cascadius loans proxy / mirror loans in real life, the lifecycle of loans on Cascadius will mirror that of loans in real life.  Delinquent loans follow the standard 30-60-90 DPD states, after which the loans are assumed defaulted and the creditor can begin liquidation and recovery processes on the loan.  The actual recovery will happen outside of Cascadius, but the recovered proceeds net of expenses will be repaid to the creditor on Cascadius.

#### Refinancing & Prepayments

Loans may be prepaid, at which point the proceeds are distributed to the securitization vehicle.  A refinancing effectively pays off the loan and originates a new loan with the remaining outstanding balance - this is operationally facilitated by the issuer or borrower, but the securitization vehicle will receive the net proceeds from the paydown.



_\*\* Note that in traditional securitizations, large loans can be partitioned across securitizations.   This is the case particularly for large commercial and corporate loans.  We'd like to keep Cascadius as simple as possible and work with the more simple assumption of non-divisibility at this time._
