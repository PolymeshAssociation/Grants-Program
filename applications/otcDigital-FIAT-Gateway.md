# Polymesh Association Grant Proposal

> This document will be part of the terms and conditions of your agreement and therefore needs to contain all the required information about the project. Don't remove any of the mandatory parts presented in bold letters or as headlines! Lines starting with a `>` (such as this one) can be removed.
>

- **Project Name:** FIAT Gateway 
- **Team Name:** otcDigital
- **Payment Address:** Polymesh (POLYX) payment address. USD 
- **Level:** 3

## Project Overview :page_facing_up:

If this application is in response to an [RFPs](https://github.com/PolymeshAssociation/Grants-Program/tree/main/rfp-proposal), please indicate this on the first line of this section.

If this is an application for a follow-up grant (the continuation of an earlier, successful Polymesh grant), please provide name and/or pull request of said grant on the first line of this section.

### Overview

Please provide the following:

- Project Name. FIAT Gateway
- A brief description of your project:    
       The FIAT Gateway provides a secure,  reliable and fully open-source middleware infrastructure to banks so they can issue FIAT tokens on Polymesh against customer bank deposits. The gateway enables banks with a 2-way channel for minting against bank deposits as well as burning fiat tokens on Polymesh with credit going to the depository accounts. 
- An indication of how your project relates to / integrates into Polymesh ecosystem.   
   The project provides a regulatory compliant way to issue, transfer and redeem FIAT tokens in Polymesh thus enabling Delivery vs Payment (DvP) for security tokens on Polymesh. 

- An indication of why your team is interested in creating this project.
  In our interactions with global banks, it became very clear that banks prefer settlement finality via atomic DvP and want to avoid any sort of settlement failures leading to huge credit risk. Banks have also indicated that they are unable to use public stablecoins such as USDC due to lack of regulatory clarity and credit risk against stablecoin providers. Hence, our solution would enable adoption of Polymesh for its security token infrastructure and the gateway's stablecoin features against bank deposits. otcDigital has built many institutional security asset classes such as bonds, commercial paper, structured notes and regulatory compliant wrapped cryptos on Polymesh. The fiat infrastructure will complete the feature set required by banks to operate and run security token marketplace using otcDigital platforms and this open source fiat gateway. 

### Project Details

We expect the teams to already have a solid idea about your project's expected final state. Therefore, we ask the teams to submit (where relevant):

- Mockups/designs of any UI components
    Please refer to otcDigital FIAT Transfer.png file for a sample UI
- Data models / API specifications of the core functionality
    The data model will be primarily based on JSON to reflect the transfer functions and the core transfer features will reflect Polymesh asset transfer functions. In addition, the model will specify the Currency, Issuer, Department, Customer ID, Customer Account fields for minting and redemption of fiat tokens. 
- An overview of the technology stack to be used
    Please refer to the otcDigital FIAT Tech Stack.png file. The technology architecture enables multiple departments within a bank can independently or collectively interact with the gateway for managing FIAT tokens. 
- Documentation of core components, protocols, architecture, etc. to be deployed
  - Core Components: Apache Kafka (open-source platform for integration with core banking systems)
  - Protocols: JMS, JSON 
      
- PoC/MVP or other relevant prior work or research on the topic.  
    In Polymesh, we have deployed and tested simple FIAT tokens such as RUSD, RGBP
   
- What your project is **_not_** or will **_not_** provide or implement
  - This is a place for you to manage expectations and to clarify any limitations that might not be obvious.
    - The gateway is stateless and hence it does not provide any historic data of prior transactions

### Ecosystem Fit

Help us locate your project in the Polymesh ecosystem / landscape and what problems it tries to solve by answering each of these questions:

- Where and how does your project fit into the ecosystem?
  - The project is a critical component to migrate hundreds of billions of institutional deposits into bank operated FIAT tokens on Polymesh 
- Who is your target audience (wallet/UI developers, designers, your own user base, yourself)?
   - Global Banks, Institutional Investors, Regional and Community Banks managing trillions of dollars of TradFi assets
- What need(s) does your project meet?
  - Atomic DvP supporting instant settlement and settlement guarantee
- Are there any other projects similar to yours in the Polymesh ecosystem?
  - Not to our knowledge. Otherwise we would have used such a feature. While we understand there is on-going discussions with other stable coin providers, these may not be workable with banks who would want to control the flow of FIAT tokens within their own desks. That's part of the reason why a pub-sub feature is included and in-addition it is expected that the FIAT gateway would be run within each bank's internal infrastructure for security reasons. 
  - If so, how is your project different?  See above
  - If not, are there similar projects in related ecosystems?  See above

## Team :busts_in_silhouette:

### Team members

- Name of team leader
  - Mani Pillai
- Names of team members
  - Jamal Mohamed
  - Vipin Bharathan

### Contact

- **Contact Name:** Full name of the contact person in your team:  Mani Pillai
- **Contact Email:** Contact email (e.g. jane@example.com): mani@otc.digital
- **Website:** Any website for your team, company, or project   otc.digital

### Legal Structure

- **Registered Address:** Address of your registered legal entity, if available. Please keep it in a single line. (e.g. High Street 1, London LK1 234, UK)  
  216 Navajo Ct, Morganville, NJ 07751, USA
- **Registered Legal Entity:** Name of your registered legal entity, if available. (e.g. Acme Ltd.)
  SwapsHub Company Inc. (doing business as otcDigital)

### Team's experience

Please describe the team's relevant experience. If your project involves development work, we would appreciate it if you singled out a few interesting projects or contributions made by team members in the past. For research-related grants, references to past publications and projects in a related domain are helpful.
   
   We have extensive experience in building and deploying large scale financial products and networks in capital markets. These range from cash equities, forwards, lending, otc derivatives to global banks such as Bank of America, Morgan Stanley, Macquarie Bank etc. 

If anyone on your team has applied for a grant previously, please list the name of the project and legal entity here.

### Team Code Repos

Provide the address of the github org and repos where the completed project will be hosted
- https://github.com/otcDigital
- https://github.com/otcDigital/fiat-gatewy
- https://github.com/<your_organisation>/<project_2>

Please also provide the GitHub accounts of all team members. If they contain no activity, references to projects hosted elsewhere or live are also fine.

- https://github.com/mmani99
- https://github.com/<team_member_2>

### Team LinkedIn Profiles (if available)

- https://www.linkedin.com/in/manipillai1/
- https://www.linkedin.com/in/jamal-mohamed-naina-mohamed-5498768/

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

> :zap: If any of your deliverables is based on somebody else's work, make sure you work and publish _under the terms of the license_ of the respective project and that you **highlight this fact in your milestone documentation** and in the source code if applicable! **Teams that submit others' work without attributing it will be immediately terminated.**

### Overview

- **Total Estimated Duration:** Duration of the whole project (e.g. 2 months)
- **Full-Time Equivalent (FTE):**  Average number of full-time employees working on the project throughout its duration (see [Wikipedia](https://en.wikipedia.org/wiki/Full-time_equivalent), e.g. 2 FTE)
- **Total Costs:** Requested amount in USD for the whole project (e.g. 12,000 USD). Note that the acceptance criteria and additional benefits vary depending on the [level](../README.md#level_slider-levels) of funding requested. This and the costs for each milestone need to be provided in USD; since the grant is paid out in POLYX, the amount will be calculated according to the exchange rate at the time of payment.

### Milestone 1 Example — Implement Substrate Modules

- **Estimated duration:** 1 month
- **FTE:**  2
- **Costs:** 8,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a. | License | Apache 2.0 / GPLv3 / MIT / Unlicense |
| 0b. | Documentation | We will provide both **inline documentation** of the code and a basic **tutorial** that explains how a user can (for example) spin up one of our Substrate nodes and send test transactions, which will show how the new functionality works. |
| 0c. | Testing Guide | Core functions will be fully covered by unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| 0d. | Docker | We will provide a Dockerfile(s) that can be used to test all the functionality delivered with this milestone. |
| 0e. | Article | We will publish an **article**/workshop that explains [...] (what was done/achieved as part of the grant). (Content, language and medium should reflect your target audience described above.)
| 1. | Feature: X | We will create a feature that will... (Please list the functionality that will be implemented for the first milestone) |  
| 2. | Feature: Y | We will create a feature that will... |  


### Milestone 2 Example — Additional features

- **Estimated Duration:** 1 month
- **FTE:**  1
- **Costs:** 4,000 USD

...


## Future Plans

Please include here

- how you intend to use, enhance, promote and support your project in the short term, and
- the team's long-term plans and intentions in relation to it.


## Additional Information :heavy_plus_sign:

**How did you hear about the Grants Program?** Polymesh Website / Medium / Twitter / Discord / Newsletter / Announcement by another team / personal recommendation / etc.

Here you can also add any additional information that you think is relevant to this application but isn't part of it already, such as:

- Work you have already done.
- If there are any other teams who have already contributed (financially) to the project.
- Previous grants you may have applied for.
