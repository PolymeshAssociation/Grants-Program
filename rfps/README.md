# Requests for Proposals

- [Requests for Proposals](#requests-for-proposals)
  - [:grey_question: What is an RFP?](#grey_question-what-is-an-rfp)
  - [:scroll: List of current RFPs](#scroll-list-of-current-rfps)
    - [Security Token Orientated Block Explorer](#security-token-orientated-block-explorer)
      - [Project Description :page_facing_up:](#project-description-page_facing_up)
    - [Hardware Wallet Integration](#hardware-wallet-integration)
      - [Project Description :page_facing_up:](#project-description-page_facing_up-1)
    - [Double Entry Accounting Style Export](#double-entry-accounting-style-export)
      - [Project Description :page_facing_up:](#project-description-page_facing_up-2)
    - [Enterprise Software Wallet Integration](#enterprise-software-wallet-integration)
      - [Project Description :page_facing_up:](#project-description-page_facing_up-3)
    - [Mobile Wallet Options for Polymesh](#mobile-wallet-options-for-polymesh)
      - [Project Description :page_facing_up:](#project-description-page_facing_up-4)
    - [Source Connector for Kafka Connect](#source-connector-for-kafka-connect)
      - [Project Description :page_facing_up:](#project-description-page_facing_up-5)


## :grey_question: What is an RFP?

An RFP (Request for Proposals) is a declaration of interest for others to submit a grant application regarding a specific project. They usually revolve around issues that the author (often someone from our team) deems useful and missing or unsolved in our ecosystem.

If you find an open RFP here that you think you can address, feel free to [submit a grant application](../README.md#1-application). There is a [section in our application template](../applications/application-template.md#project-overview-page_facing_up) where you can reference the RFP you are addressing.

## :scroll: List of current RFPs

### Security Token Orientated Block Explorer

- [:arrow_right: finance-orientated-block-explorer.md](./finance-orientated-block-explorer.md)
- **Proposer:** Polymath Research

#### Project Description :page_facing_up:

A chain explorer that is orientated to our exact data, showing assets, settlements, identity based data.

**Business Rationale:** Moves away from the generic Subscan based explorer to something that leverages our layer 1 data more directly. Possible starting point for a reporting portal.

**Approximate time (person week):** 8 weeks

**Impacted Components:** SubQuery / GraphQL possibly.

----

### Hardware Wallet Integration

- [:arrow_right: hardware-wallet-integration.md](./hardware-wallet-integration.md)
- **Proposer:** Polymath Research

#### Project Description :page_facing_up:

Integrate Polymesh with additional hardware wallets (e.g. non-Ledger models).

**Business Rationale:** Provide more options to users for securing private keys.

**Approximate time (person week):** 6 weeks.

**Impacted Components:** Core Schema.

----

### Double Entry Accounting Style Export

- [:arrow_right: double-entry-accounting-style-export.md](./double-entry-accounting-style-export.md)
- **Proposer:** Polymath Research

#### Project Description :page_facing_up:

Report export (or maybe integration to something like Quickbooks/Freshbooks etc) to record transactions as full double entry accounting style ledgers. Example:  [Bitcoin app for QuickBooks](https://blockpath.com/apps/qb/features?realmId=&channel=appscom).

**Business Rationale:** Assist with financial reporting for investors.

**Approximate time (person week):** 6 weeks + 2 weeks per integration.

**Impacted Components:** Core / SubQuery.

----

### Enterprise Software Wallet Integration

- [:arrow_right: enterprise-software-wallet-integration.md](./enterprise-software-wallet-integration.md)
- **Proposer:** Polymath Research

#### Project Description :page_facing_up:

Add Polymesh support to the API one of enterprise wallets like [Zumo](https://developers.zumo.money/docs/).

**Business Rationale:** Provide more ways to onboard new users and provide a fiat on-ramp.

**Approximate time (person week):** 6 weeks.

**Impacted Components:** Core, and maybe more towards general key management integrations.

----

### Mobile Wallet Options for Polymesh 

- [:arrow_right: walletconnect-for-substrate.md](./walletconnect-for-substrate.md)
- **Proposer:** Polymath Research

#### Project Description :page_facing_up:

Approaches like WalletConnect allow a dApp to delegate transaction signing to any arbitrary wallet, including mobile wallets, via QR codes and direct communication with the wallet.

This broadens the range of wallets that could be used with Polymesh dApps giving users more choices for how to secure their private keys.

**Business Rationale:** Allows a broader range of wallet solutions, including both custodial, MPC-based and self-custodial.

**Approximate time (person week):** 12 weeks.

**Impacted Components:** Tooling.

----

### Source Connector for Kafka Connect

- [:arrow_right: source-connector-for-kafka-connect.md](./source-connector-for-kafka-connect.md)
- **Proposer:** Polymath Research

#### Project Description :page_facing_up:

This allows to stream all events from Polymesh to Kafka systems. It can be then transformed, stored, accessed from many other systems.

As an example in case of Polymath, one of the use cases would be current GraphQL implementation. At the moment it uses dedicated software that gets the data from the blockchain, saves it to a postgresql db and from there it can be accessed as GraphQL endpoint. If there is any other use case to use the full chain data, there is a high chance we would need to build that new solution from scratch, and we would have another system that synchronizes with the blockchain.

Kafka as a source of truth could be used by any number of applications. It also supports schema evolution so there is a chance we would not have to resync everything from scratch each time an update is made.

Other companies could use that for whatever use cases they can think of, so for instance a token issuer could configure the connector to subscribe to events related to their tokens only.

**Business Rationale:** Apache Kafka is most widely used messaging platform that can be used as a single source of truth for all data in a company. 

**Approximate time (person week):** 2 weeks.

**Impacted Components:** SubQuery / GraphQL possibly.

----
