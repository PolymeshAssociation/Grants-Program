# Polymesh Association Grant Proposal

- **Project Name:** FIAT Gateway 
- **Team Name:** otcDigital
- **Payment Address:** Polymesh (POLYX) payment address. Currency: USD 
- **Level:** 3

## Project Overview :page_facing_up:

If this application is in response to an [RFPs](https://github.com/PolymeshAssociation/Grants-Program/tree/main/rfp-proposal), please indicate this on the first line of this section.

If this is an application for a follow-up grant (the continuation of an earlier, successful Polymesh grant), please provide name and/or pull request of said grant on the first line of this section.

### Overview

Please provide the following:

- Project Name.   **FIAT Gateway**
- A brief description of your project:    

The FIAT Gateway provides a secure,  reliable and fully open-source middleware infrastructure to banks so they can issue FIAT stable tokens on Polymesh against customer bank deposits. The gateway enables banks with a 2-way channel for minting against bank deposits as well as burning fiat tokens on Polymesh with credit going to the depository accounts. 

- An indication of how your project relates to / integrates into Polymesh ecosystem.   

The project provides a regulatory compliant way to issue, transfer and redeem FIAT tokens in Polymesh thus enabling Delivery vs Payment (DvP) for security tokens on Polymesh. Unlike public stablecoins, these tokens are managed by banks against their customer deposits and hence can meet regulatory compliance. 

- An indication of why your team is interested in creating this project.  

In our interactions with global banks, it became very clear that banks prefer settlement finality via atomic DvP and want to avoid any sort of settlement failures leading to huge credit risk. Banks have also indicated that they are unable to use public stablecoins such as USDC due to lack of regulatory clarity and credit risk against stablecoin providers. Hence, our solution would enable adoption of Polymesh for its security token infrastructure and the gateway's stable token features against bank deposits. otcDigital has built several institutional security asset classes such as bonds, commercial paper, structured notes and regulatory compliant wrapped cryptos on Polymesh. The fiat infrastructure will complete the feature set required by banks to operate and run security token marketplace using otcDigital or third party platforms. 

### Project Details

We expect the teams to already have a solid idea about your project's expected final state. Therefore, we ask the teams to submit (where relevant):

- Mockups/designs of any UI components  

Please refer to the **otcDigital FIAT Transfer.png** file for a sample UI  
<img src="otcDigital FIAT Transfer.png" />

- Data models / API specifications of the core functionality  

The data model will be primarily based on JSON to reflect the transfer functions and the core transfer features will reflect Polymesh asset transfer functions. In addition, the model will specify the Currency, Issuer, Department, Customer ID, Customer Account fields for minting and redemption of fiat tokens. 
- An overview of the technology stack to be used  

Please refer to the **FIAT Gateway Tech stack.png** file. <img src="FIAT Gateway Tech stack.png" />
The tech stack consists of Polymesh local with relayer, HashiCorp Vault for development specific key management, otc fiat gateway, Apache Kafka for pub-sub events between banks and their customers. The technology architecture enables multiple departments within a bank can independently or collectively interact with the gateway for managing FIAT tokens. 
- Documentation of core components, protocols, architecture, etc. to be deployed

Core Components: Gateway services written in Kotlin, Java. Apache Kafka (open-source platform for integration with core banking systems), HashiCorp Vault for basic Polymesh key management, Polymesh Relayer docker service for connecting to the Polymesh Node

Protocols: JMS, JSON 
      
- PoC/MVP or other relevant prior work or research on the topic.  

In Polymesh, we have deployed and tested simple FIAT tokens such as RUSD, RGBP
   
- What your project is **_not_** or will **_not_** provide or implement
  - This is a place for you to manage expectations and to clarify any limitations that might not be obvious.  

    - The gateway is stateless and hence it does not provide any historic data of prior transactions
    - No UI will be provided as the gateway is a service
    - No core banking functions regarding FIAT accounts will be provided

### Ecosystem Fit

Help us locate your project in the Polymesh ecosystem / landscape and what problems it tries to solve by answering each of these questions:

- Where and how does your project fit into the ecosystem?  

The project is a critical component to migrate trillions of US dollars of institutional deposits into bank operated FIAT tokens on Polymesh 

- Who is your target audience (wallet/UI developers, designers, your own user base, yourself)?  

Global Banks, Institutional Investors, Regional and Community Banks managing trillions of dollars of TradFi assets
- What need(s) does your project meet?  

Atomic DvP supporting instant settlement and settlement guarantee

- Are there any other projects similar to yours in the Polymesh ecosystem?  

Not to our knowledge. Otherwise we would have used such a feature. While we understand there is on-going discussions with other stable coin providers, these may not be workable with banks who would want to control the flow of FIAT tokens against customer deposit accounts and within their own desks. That's part of the reason why a multi-desk pub-sub feature is included and in-addition it is expected that the FIAT gateway would be run within each bank's internal infrastructure for security reasons. 

  - If so, how is your project different?  
  
See above
  - If not, are there similar projects in related ecosystems?  
  
See above

## Team :busts_in_silhouette:

### Team members

- Name of team leader
  - Mani Pillai
- Names of team members
  - Jamal Mohamed
  - Vipin Bharathan

### Contact

- **Contact Name:** Full name of the contact person in your team:  Mani Pillai
- **Contact Email:** mani@otc.digital
- **Website:** Any website for your team, company, or project   otc.digital

### Legal Structure

- **Registered Address:** Address of your registered legal entity, if available. Please keep it in a single line. (e.g. High Street 1, London LK1 234, UK)  

216 Navajo Ct, Morganville, NJ 07751, USA

- **Registered Legal Entity:** Name of your registered legal entity, if available. (e.g. Acme Ltd.)  

SwapsHub Company Inc. (doing business as otcDigital)

### Team's experience

Please describe the team's relevant experience. If your project involves development work, we would appreciate it if you singled out a few interesting projects or contributions made by team members in the past. For research-related grants, references to past publications and projects in a related domain are helpful.  
   
<i>We have extensive experience in building and deploying large scale financial products and networks in capital markets. These range from cash equities, forwards, lending, otc derivatives to global banks such as Bank of America, Morgan Stanley, Macquarie Bank etc. </i>

If anyone on your team has applied for a grant previously, please list the name of the project and legal entity here.  

None


### Team Code Repos

Provide the address of the github org and repos where the completed project will be hosted
- https://github.com/otcDigital
- https://github.com/otcDigital/fiat-gateway

Please also provide the GitHub accounts of all team members. If they contain no activity, references to projects hosted elsewhere or live are also fine.

- https://github.com/mmani99
- https://github.com/nmjamal
- https://github.com/vipinsun

### Team LinkedIn Profiles (if available)

- https://www.linkedin.com/in/manipillai1/
- https://www.linkedin.com/in/jamal-mohamed-naina-mohamed-5498768/
- https://www.linkedin.com/in/vipin-bharathan/

## Development Status :open_book:

If you've already started implementing your project or it is part of a larger repository, please provide a link and a description of the code here. In any case, please provide some documentation on the research and other work you have conducted before applying. This could be:

- links to improvement proposals or [RFPs](https://github.com/PolymeshAssociation/Grants-Program/tree/main/rfp-proposal) (requests for proposal),
- academic publications relevant to the problem,
- links to your research diary, blog posts, articles, forum discussions or open GitHub issues,
- references to conversations you might have had related to this project with anyone from the Web3 Foundation,
- previous interface iterations, such as mock-ups and wireframes.  

Please refer to the diagrams uploaded and the architecture described above.


## Development Roadmap :nut_and_bolt:

This section should break the development roadmap down into milestones and deliverables. To assist you in defining it, we have created a document with examples for some grant categories [here](../docs/grant_guidelines_per_category.md). Since these will be part of the agreement, it helps to describe _the functionality we should expect in as much detail as possible_, plus how we can verify and test that functionality. Whenever milestones are delivered, we refer to this document to ensure that everything has been delivered as expected.

Below we provide an **example roadmap**. In the descriptions, it should be clear how your project is related to Polymesh. We _recommend_ that teams structure their roadmap as 1 milestone ≈ 1 month. We also _recommend_ that you build up the scope of the project in a way that it can be completed in max 3 months. If the entirety of your project is going to take more than 3 months, please submit it's parts that can be completed in 3 months as one grant project. This helps us move forward quickly and deliver features quickly.

For each milestone,

- make sure to include a specification of your software. _Treat it as a contract_; the level of detail must be enough to later verify that the software meets the specification.
- include the amount of funding requested _per milestone_.
- include documentation (tutorials, API specifications, architecture diagrams, whatever is appropriate) in each milestone. This ensures that the code can be widely used by the community.
- provide a test suite, comprising unit and integration tests, along with a guide on how to set up and run them.
- commit to providing Dockerfiles for the delivery of your project.
- indicate milestone duration as well as number of full-time employees working on each milestone.
- **Deliverables 0a-0d are mandatory for all milestones**, and deliverable 0e at least for the last one. If you do not intend to deliver one of these, please state a reason in its specification (e.g. Milestone X is research oriented and as such there is no code to test).

### Overview

- **Total Estimated Duration:** Duration of the whole project: **5 months**
- **Full-Time Equivalent (FTE):**  Average number of full-time employees working on the project throughout its duration (see [Wikipedia](https://en.wikipedia.org/wiki/Full-time_equivalent), e.g. 2 FTE)   **2 FTE**
- **Total Costs:** Requested amount in USD for the whole project (e.g. 12,000 USD). Note that the acceptance criteria and additional benefits vary depending on the [level](../README.md#level_slider-levels) of funding requested. This and the costs for each milestone need to be provided in USD; since the grant is paid out in POLYX, the amount will be calculated according to the exchange rate at the time of payment.  
**USD 240,000**

### Milestone 1 — Initial Documentation

- **Estimated duration:** 1 month
- **FTE:**  2
- **Costs:** 40,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a. | License | Apache 2.0 |
| 0b. | Documentation | We will provide both **inline documentation** of the code and a basic **tutorial** that explains how a user can (for example) spin up our gateway and send test transactions, which will show how the new functionality works. |
| 0c. | Testing Guide | Core functions will be fully covered by unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| 0d. | Docker | We will provide a Dockerfile(s) that can be used to test all the functionality delivered with this milestone. |
| 0e. | Article | We will publish an **article** on linkedIn that explains the virtues of the gateway.
| 1. | Infrastructure Setup Documentation | We will provide an outline document to setup components such as Apache Kafka, HashiCorp Vault, Polymesh Local |  
| 2. | Apache Kafka Setup | We will create Apache Kafka infrastructure for the developement environment |  
| 3. | HashiCorp Vault Setup | The Vault infrastructure will be setup for development environment |  
| 4. | Polymesh Local Setup | The latest Polymesh Local docker infrastructure will be setup for development environment |  


### Milestone 2 — Configuration and testing scripts

- **Estimated Duration:** 1 month
- **FTE:**  2
- **Costs:** 50,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a to 0d. | License, Docs, Testing, etc. | As in Milestone 1 |
| 1. | Kafka configuration scripts | We will create scripts to setup Kafka and event channels |  
| 2. | Vault configuration scripts | We will create scripts to setup HashiCorp Vault with appropriate commands for setting up transit engine and key names |  
| 3. | Vault test scripts | We will provide a set of scripts to test the vault features required for managing the keys for FIAT tokens |  
| 4. | Kafka pub/sub test programs | We will provide a set of programs to publish and subscribe to the specific event channels |  
| 5. | Gateway Service Setup | The gateway service will be built using Open-source IntelliJ IDEA, Kotlin/Java. All application unit tests will be available under the IDEA platform. A project gradle build file will be provided  |  
  
  
  
### Milestone 3 — FIAT to Poly Stable Token Issuance 

- **Estimated Duration:** 1 month
- **FTE:**  2
- **Costs:** 50,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a to 0d. | License, Docs, Testing, etc. | As in Milestone 1 |
| 1. | FIAT to Poly tokens JSON | All relevant Jsons will be finalized for this service |  
| 2. | Gateway Function: Integration with Polymesh | The gateway service will be integrated with Polymesh local |  
| 4. | Gateway Issue Function | The issue function in the gateway will be implemented to interact with Polymesh that enables issuance of FIAT equivalent Poly stable tokens. |  
| 3. | Gateway Transfer Function | The transfer function in the gateway will be implemented to interact with Polymesh that enables transfer of Poly stable tokens between wallets. |  
| 4. | Kafka client API to request FIAT conversion | The API will be implemented to request the issuer for FIAT to Poly token conversion |  
| 5. | Kafka client API to request issue of Poly FIAT tokens | The API will be implemented to request Poly token issuance (minting) |  
| 6. | Kafka client API to transfer of Poly FIAT tokens | The API will be implemented to transfer Poly tokens between parties |  
| 7. | Test scripts | The test scripts for the above issuance features will be implemented and tested |  


### Milestone 4 — Poly Stable Token Redemption 

- **Estimated Duration:** 1 month
- **FTE:**  2
- **Costs:** 50,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a to 0d. | License, Docs, Testing, etc. | As in Milestone 1 |
| 1. | Poly stable tokens to FIAT JSON | All relevant Jsons will be finalized for this service |  
| 2. | Gateway Redemption Function | The redemption function in the gateway will be implemented to interact with Polymesh that enables redemption of Poly tokens. |  
| 3. | Kafka client API to request FIAT redemption | The API will be implemented to request issuer to redeem Poly tokens and convert to FIAT position|  
| 4. | Kafka Bank API to request Poly token redemption | The API will be implemented for issuer to request redemption of Poly tokens |  
| 5. | Test scripts | The test scripts for the above redemption features will be implemented and tested |  

### Milestone 5 — Full integration, testing and delivery 

- **Estimated Duration:** 1 month
- **FTE:**  2
- **Costs:** 50,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a to 0d. | License, Docs, Testing, etc. | As in Milestone 1 |
| 1. | Client test program for bank customer | This test program should be able to request issuance and redemption of Poly stable tokens with the FIAT gateway service |  
| 2. | Bank/Issuer test program | This test program should enable a bank to request issuance, transfer and redeem Poly stable tokens against FIAT positions |  
| 3. | Client integration testing doc| A document will be outlined to perform client integration and testing the life-cycle features |  
| 4. | Bank integration testing doc| A document will be outlined to perform bank integration and testing the life-cycle features |  
| 5. | Final Release to Polymesh Repo| The completed project will all source code, documentation, test scripts etc. will be committed to the Polymesh repo at the prescribed directory |  


## Future Plans

Please include here

- how you intend to use, enhance, promote and support your project in the short term, and
- the team's long-term plans and intentions in relation to it.

  Along with the open-source gateway work, otcDigital intends to integrate its platform and network with the gateway for a full product demo to banks and other financial institutions. otcDigital also actively markets its solutions based on Polymesh to potential adopters of security tokens. 
  Based on further inputs from market participants, otcDigital intends to further develop and enhance to add other capabilities such as compliance, regulatory reporting etc. 

## Additional Information :heavy_plus_sign:

**How did you hear about the Grants Program?** Polymesh Website / Medium / Twitter / Discord / Newsletter / Announcement by another team / personal recommendation / etc.

  otcDigital has been working with Polymesh for more than 18 months on building enterprise security token solutions. We learnt about the Grants program through our regular course of interactions with Polymesh / Polymath teams. 

Here you can also add any additional information that you think is relevant to this application but isn't part of it already, such as:

- Work you have already done.  

     otcDigital has built a whole ecosystem of trading platforms and network for all market participants: buy-side, sell-side and custodians. It intends to integrate the gateway with the otcDigital platform and offer it as part of its overall solution. 

- If there are any other teams who have already contributed (financially) to the project.

  None

- Previous grants you may have applied for.  

  No provious grants were applied. 
