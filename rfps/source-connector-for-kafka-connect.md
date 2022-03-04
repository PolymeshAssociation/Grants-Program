# Source Connector for Kafka Connect 

* **Proposer:** [Polymath Research](https://polymath.network)
* **Status:** Open

## Project Description :page_facing_up: 

This allows to stream all events from Polymesh to Kafka systems. It can be then transformed, stored, accessed from many other systems.

As an example in case of Polymath, one of the use cases would be current GraphQL implementation. At the moment it uses dedicated software that gets the data from the blockchain, saves it to a postgresql db and from there it can be accessed as GraphQL endpoint. If there is any other use case to use the full chain data, there is a high chance we would need to build that new solution from scratch, and we would have another system that synchronizes with the blockchain.

Kafka as a source of truth could be used by any number of applications. It also supports schema evolution so there is a chance we would not have to resync everything from scratch each time an update is made.

Other companies could use that for whatever use cases they can think of, so for instance a token issuer could configure the connector to subscribe to events related to their tokens only.

**Business Rationale:** Apache Kafka is most widely used messaging platform that can be used as a single source of truth for all data in a company. 

**Approximate time (person week):** 2 weeks.

**Impacted Components:** SubQuery / GraphQL possibly.
