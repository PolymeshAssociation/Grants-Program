# docIT bot Integration for Polymesh

- **Team Name:** DocIT
- **Payment Address:** 2EKMC24PB5Mkk7HVzqPjTtGmpMR2vJRFmXUfp1FG3T79mbvY (POLYX)
- **Level:** 1

## Project Overview :page_facing_up:

### Overview

- **Tagline:** "Converse with Polymesh Documentation"
- **Description:** We propose "docIT," a Discord bot designed to provide users with a conversational interface to access Polymesh's documentation and repositories. Harnessing the latest Large Language Models (LLMs), docIT aims to interconnect Polymesh's essential GitHub repositories, documentation, articles, and forums.
- **Integration:** Our bot will seamlessly integrate with the Polymesh ecosystems, providing a bridge between users and essential technical resources.
- **Interest:** Our team recognizes the growth and active community of Polymesh. By enhancing accessibility and user experience, we aim to further foster community growth and developer engagement.

### Project Details

- **UI Components:** The primary interface will be via Discord, with potential expansion to other chat platforms in the future. Happy to integrate with Element if needed.
- **Data Models/API:** We'll use OpenAI's GPT to interpret user queries and fetch relevant documentation sections.
- **Technology Stack:** OpenAI for language processing, Node.js for backend operations, and Discord API for bot integration.
- **Documentation:** Comprehensive documentation will cover bot interactions, command structures, and integration processes.
- **Prior Work:** Our team has previously developed chatbots for other blockchain platforms, demonstrating our expertise.
- **Limitations:** The bot will focus on documentation retrieval and won't handle transactional or wallet operations.

### Ecosystem Fit

- **Fit:** docIT serves as a bridge between the Polymesh communities and their respective documentation.
- **Target Audience:** Developers, enthusiasts, and newcomers within the Polymesh ecosystems.
- **Needs Met:** Streamlined access to technical resources and improved community engagement.
- **Similar Projects:** While there are bots for community management, none focus on documentation retrieval for Polymesh.

## Team :busts_in_silhouette:

### Team members

- Nigel Alford (owner/developer)

### Contact

- **Contact Name:** Nigel Alford
- **Contact Email:** ngalford@gmail.com
- **Website:** https://docIT.cc

### Legal Structure

- **Registered Address:** N/A

### Team's experience

Our team has experience in blockchain technology, having developed tools for blockchains like Ethereum and Tezos. Notably, our Tezos-based chatbot and NFT Marketplace was widely adopted by its community. Nigel Alford has been a web developer for 10+ years.

### Team Code Repos

- https://github.com/mrnigelalford/docit-discord
- https://github.com/mrnigelalford

### Team LinkedIn Profiles 

- https://www.linkedin.com/in/nigelalford

## Development Status :open_book:

Our team has laid the groundwork for the bot, with a prototype demonstrating basic interactions. We've also conducted preliminary research into Polymesh's documentation structures.

### Development Roadmap :nut_and_bolt:

### Overview

- **Total Estimated Duration:** 4 weeks
- **Full-Time Equivalent (FTE):** 3
- **Total Costs:** 8,000 USD

## Backend Development

### Requirements
Language: Typescript | Node.js
Database: Supabase | self-hosted docker files
Hosting location: Digital Ocean
Scaling: Increased instance sizes will be utilized. If needed, will setup shared instances across VMs to balance load.
CI/CD: Github Actions into Digital Ocean
All secrets stored in environment variables
Data Sources: Documentation, primary repo, open to pulling chat history or other sources if needed.

## UI Development
App will front to Discord Bot
Commands: Direct mention docIT with a question. DocIT will respond in a thread with response. All additional communications can exist in a threaded conversation.
Happy to create more commands or interactions if needed.

### Pre-Implementation

Before diving into the milestones, we will collaborate with the Polkadot teams. Our goal is to understand their needs deeply, pinpoint areas of concern, and determine where our bot can provide the most value. The insights from these sessions will guide our choice of data sources for the following milestones.

### Milestone 1 Example — Basic functionality

- **Estimated duration:** 1 month
- **FTE:**  1,5
- **Costs:** 8,000 USD

> :exclamation: **The default deliverables 0a-0d below are mandatory for all milestones**, and deliverable 0e at least for the last one. 

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **0a.** | License | Apache 2.0 / GPLv3 / MIT / Unlicense |
| **0b.** | Documentation | We will provide both **inline documentation** of the code and a basic **tutorial** that explains how a user can (for example) spin up one of our Substrate nodes and send test transactions, which will show how the new functionality works. |
| **0c.** | Testing and Testing Guide | Core functions will be fully covered by comprehensive unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| **0d.** | Docker | We will provide a Dockerfile(s) that can be used to test all the functionality delivered with this milestone. |
| 0e. | Article | We will publish an **article**/workshop that explains [...] (what was done/achieved as part of the grant). (Content, language and medium should reflect your target audience described above.) |
| 1. | Substrate module: X | We will create a Substrate module that will... (Please list the functionality that will be implemented for the first milestone. You can refer to details provided in previous sections.) |
| 2. | Substrate module: Y | The Y Substrate module will... |
| 3. | Substrate module: Z | The Z Substrate module will... |
| 4. | Substrate chain | Modules X, Y & Z of our custom chain will interact in such a way... (Please describe the deliverable here as detailed as possible) |
| 5. | Library: ABC | We will deliver a JS library that will implement the functionality described under "ABC Library" |
| 6. | Smart contracts: ... | We will deliver a set of ink! smart contracts that will...


### Milestone 1 — Implementation of Data Sources 

- **Estimated duration:** 2 weeks
- **FTE:** 2
- **Costs:** 4,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **0a.** | License | MIT |
| **0c.** | Data Crawling | Extracting relevant data from the identified sources. |
| **0d.** | OpenAI Embeddings | Create embeddings using OpenAI, indexing them for efficient search on user queries. |
| 1. | Data Source Integration | Refine file loading, index creation, and seamlessly integrate the selected data sources into the bot. |

**End state:** A bot that can query 3-4 integrated data sources.
**Expected bugs:** Potential hallucinations and mismatches between queries and documents.

### Milestone 2 — Testing, Optimization, and Deployment

- **Estimated Duration:** 2 weeks
- **FTE:** 2
- **Costs:** 4,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **0a.** | License | MIT |
| 1. | Hallucination Mitigation | Techniques to reduce and eliminate hallucinations from bot responses. |
| 2. | Prompt Engineering | Refine the bot's prompting to ensure it provides only relevant and accurate answers. |
| 3. | Deployment | Make the bot production-ready and deploy it to Circle's Discord page. |

**End state:** A fully functional, production-ready bot, vetted and approved by the Customer/Community Support teams, and actively deployed on Circle's Discord page.

## Future Plans

Short-term, we plan to refine and expand the bot's capabilities based on community feedback. Long-term, we envision integrating docIT with other platforms and becoming the go-to solution for documentation retrieval in the blockchain space.

## Additional Information :heavy_plus_sign:

**How did you hear about the Grants Program?** Web3 Foundation Website

- Our team has already built a foundational prototype.
- We have collaborated with the Tezos community on a similar initiative.
- This is our first grant application for the Web3 Foundation.