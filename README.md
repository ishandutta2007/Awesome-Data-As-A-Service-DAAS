# Awesome-Data-As-A-Service-DAAS

# Awesome-Data-As-A-Service-DAAS

**Top Data As A Service DAAS (Opensource) 🌟 Star if you like it! 🌟**



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Data Marketplaces, Firmographic Data Enrichment, Identity Resolution & External Data Activation*

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Data-as-a-Service (DaaS)**. These tools enable organizations to buy, sell, enrich, and activate external data—from fully managed enterprise data marketplaces with pre-packaged firmographic, contact, and financial datasets to self-hosted platforms that give teams complete control over data monetization, licensing, and privacy-preserving access.



**Examples** include Snowflake Data Marketplace, Databricks Marketplace, ZoomInfo, Clearbit, People Data Labs, Enigma, Coresignal, Crunchbase Enterprise, Experian Data Quality, and Workday Data As A Service (the category leaders in commercial space).



**Open-source emphasis**: This section is expanded with every relevant project for self-hosting, data marketplaces, and open data infrastructure. **Critical note**: True open-source DaaS platforms—where external data is packaged, licensed, and delivered as a service—are extremely sparse. Most projects below are marketplace infrastructure, SDKs, or narrow data collection tools rather than full DaaS products.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Snowflake Data Marketplace](https://www.snowflake.com/)**

  **Cloud data marketplace** integrated with Snowflake's data cloud. Provides access to third-party datasets from providers including S&P Global, Thomson Reuters, and Bright Data, with native governance and sharing controls . **Pricing**: Consumption-based (Snowflake credits) plus provider-specific data costs; quote-based. **Free tier**: Trial credits available. **Best for**: organizations already on Snowflake wanting to discover and access external datasets without data movement.



- **[Databricks Marketplace](https://www.databricks.com/)**

  **Open data marketplace** integrated with the Databricks lakehouse. **Pricing**: Consumption-based (DBUs) plus provider listings; quote-based. **Free tier**: Community Edition limited. **Best for**: data teams on Databricks wanting to combine external datasets with internal lakehouse analytics.



- **[ZoomInfo](https://www.zoominfo.com/)**

  **B2B contact and company intelligence platform** with extensive firmographic and technographic data. **Pricing**: Quote-only; annual contracts typical. **Free tier**: Limited trial available. **Best for**: sales and marketing teams needing broad B2B prospecting and enrichment data.



- **[Clearbit](https://clearbit.com/)** (HubSpot)

  **Data enrichment and intelligence API** for company and person data. **Pricing**: Usage-based API pricing; quote for enterprise. **Free tier**: Limited free tier for basic lookups. **Best for**: product and growth teams wanting real-time enrichment via API.



- **[People Data Labs](https://www.peopledatalabs.com/)**

  **Person and company data enrichment API** with a large global dataset. **Pricing**: Credit-based API pricing; quote for volume. **Free tier**: Trial credits available. **Best for**: developers and data teams wanting flexible API access to people and company data.



- **[Enigma](https://www.enigma.com/)**

  **Financial and business data intelligence** focused on SMB and merchant data. **Pricing**: Quote-only. **Free tier**: None. **Best for**: financial services and fintech companies needing verified business data.



- **[Coresignal](https://www.coresignal.com/)**

  **Public web data API** for company and employee data. **Pricing**: Credit-based API pricing. **Free tier**: Trial available. **Best for**: data teams wanting fresh, structured public web data via API.



- **[Crunchbase Enterprise](https://www.crunchbase.com/)**

  **Private company and funding data platform** for market intelligence. **Pricing**: Quote-only for enterprise; self-serve tiers available. **Free tier**: Limited free access. **Best for**: investors, analysts, and sales teams tracking startups and private markets.



- **[Experian Data Quality](https://www.experian.com/)**

  **Data quality and enrichment services** for customer and business data. **Pricing**: Quote-only. **Free tier**: None. **Best for**: enterprises needing data validation, cleansing, and enrichment at scale.



- **[Workday Data As A Service](https://www.workday.com/)**

  **Data services within the Workday ecosystem** for HR and finance data. **Pricing**: Quote-only; bundled with Workday suite. **Free tier**: None. **Best for**: Workday customers wanting governed access to Workday data for analytics and integrations.



## Open-Source GitHub Projects



- **[Unified Data Marketplace (UDAM)](https://github.com/data-agent-marketplace/data-agent-marketplace)**

  **Open-source, API-first data marketplace backend** (license per repo) — **the closest open-source match to a DaaS marketplace infrastructure** for monetizing data services. **Features**: Listings for data services and APIs, Stripe payment integration (or instant tokens for small orders), AES-256 encrypted token issuance, concurrency-safe order processing with PostgreSQL row locks, session-based auth with OAuth support, and Docker-ready deployment . **Tech stack**: Node.js/Express (backend), Next.js (minimal UI), PostgreSQL 16, Stripe. **Deploy**: Docker Compose or manual (Node.js 18+, PostgreSQL). **Trade-off**: **Marketplace infrastructure only**—you bring your own data services and listings; no pre-packaged datasets, enrichment APIs, or identity resolution. **Best for**: developers or data providers wanting to operate their own data marketplace with payment and token management built in.



- **[Ocean Enterprise](https://github.com/oceanprotocol/ocean.py)**

  **Open-source enterprise data ecosystem for monetizing AI and data products** (Apache 2.0 per Ocean Protocol ecosystem) — **the most sophisticated open-source DaaS-adjacent platform** with privacy-preserving access controls. **Features**: Publish data services as Data NFTs (ERC721) with Datatokens (ERC20) for access; **Compute-to-Data (C2D)** enables buyers to run compute against private data without the data leaving the premises—only results are visible; domain-agnostic and used in aerospace, agriculture, manufacturing, mobility, and smart cities . **Tech stack**: Python (ocean.py), blockchain (Ethereum-compatible), decentralized storage (Filecoin, Arweave, AWS, Azure). **Deploy**: Self-hosted; requires blockchain wallet and data storage setup. **Trade-off**: **Blockchain-dependent architecture**—steep learning curve, crypto wallet management, and decentralized infrastructure requirements. Not a turnkey SaaS replacement. **Best for**: organizations with sensitive or proprietary data wanting to monetize access while preserving privacy via Compute-to-Data.



- **[daas-sdk (Rust)](https://docs.rs/crate/daas/0.2.2/source/README.md)**

  **Data-as-a-Service SDK for implementing the DaaS pattern with Privacy by Design** (Apache 2.0) — **a developer toolkit for building DaaS microservices**, not a marketplace or data product. **Features**: Enablers for DaaS architecture patterns, local storage for listener services, Kafka brokering as an independent thread, processor service traits for custom data processors, and a Genesis processor for raw data flow management . **Tech stack**: Rust (Cargo). **Deploy**: Embedded in Rust applications. **Trade-off**: **SDK only**—no marketplace, no data listings, no payment infrastructure. Requires deep Rust development to build a working DaaS product. **Best for**: Rust developers building custom DaaS microservices with privacy-by-design principles baked in.



- **[PortalJS](https://github.com/datopian/portaljs)**

  **AI-native framework for building data portals** (MIT) — **the most mature open-source data portal framework** with ~2,300 GitHub stars . **Features**: Scaffold a full data portal from a brief; load datasets in minutes with agentic skills; backend-agnostic (CKAN, GitHub, Frictionless); built by Datopian, the team behind the world's first open data portals . **Tech stack**: TypeScript, Next.js. **Deploy**: Self-hosted or Datopian's Data Portal as a Service (SaaS). **Trade-off**: **Data portal framework**—for publishing and sharing datasets (open data, internal catalogs), not for selling external data or enrichment APIs. **Best for**: governments, NGOs, and organizations wanting to publish and share datasets openly or internally, not monetize third-party data.



- **[Company Atlas](https://github.com/CoreSheep/company-atlas)**

  **Unified firmographic data platform with open-source datasets** (license per repo) — **a data product, not a DaaS platform**. **Features**: Downloads Fortune 1000 company data from Kaggle, aggregates firmographic information into a unified platform; includes data collection pipelines using Kaggle API and web scraping (httpx, BeautifulSoup, trio) . **Tech stack**: Python. **Deploy**: Self-hosted (pipeline scripts). **Trade-off**: **Narrow scope** (Fortune 1000 only), no API for external consumers, no licensing or monetization features. **Best for**: researchers and developers wanting a starting point for firmographic data aggregation, not a production DaaS offering.



- **[signalforge-cli](https://pypi.org/project/signalforge-cli/)**

  **CLI tool for harvesting participant and lead data from Devpost and dev.to** (license per repo) — **a data collection utility, not a DaaS platform**. **Features**: Scrapes hackathon participant lists from Devpost, extracts author GitHub usernames from dev.to challenges, enriches emails via GitHub, and emits leads to Customer.io . **Tech stack**: Python. **Deploy**: CLI (`pip install signalforge-cli`). **Trade-off**: **Narrow, event-specific data collection** with ethical/ToS considerations; not a general-purpose DaaS product. **Best for**: developer-focused companies wanting to identify hackathon participants and dev.to challenge submitters for outreach.



### Additional Strong Open-Source Options



- **Data Fair** — Open-source platform for data sharing, visualization, and open data portals (license per repo). Used by French local governments, ADEME, EDF, and La Poste for open data and internal data marketplaces . **Note**: Primarily a **data portal and visualization platform** for public sector open data, not a commercial DaaS marketplace with paid external datasets. **Best for**: public sector and organizations wanting to publish and visualize datasets openly .

- **agent-marketplace-mcp** — MCP server for an agent-facing data marketplace (MIT). Connects AI agents to data providers for finance, satellite, agriculture, weather, geo, and research data . **Note**: **Early-stage, credits not yet purchasable**—requests are queued for evaluation. **Best for**: developers wanting to experiment with agent-driven data purchasing via MCP.

- **langchain-mart** — LangChain toolkit for LinkedIn data enrichment via Mart API (pre-release). **Note**: **Commercial API wrapper**, not open-source data infrastructure—requires Mart API key and credits . **Best for**: developers building AI agents that need LinkedIn profile and company enrichment.



**Frameworks for building custom systems**: Combine **UDAM** as marketplace infrastructure for buying and selling data services with **Ocean Enterprise** for privacy-preserving Compute-to-Data access, **PortalJS** for publishing open or internal data catalogs, and **daas-sdk** for building custom DaaS microservices in Rust—creating a DaaS stack matched to each organization's monetization model and privacy requirements.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- DaaS platforms handling personal, financial, and business data must comply with data protection regulations (GDPR, CCPA, etc.), data licensing terms, and industry-specific regulations (FCRA for credit data, HIPAA for health data).

- **The "data marketplace infrastructure" vs. "data product" vs. "data portal" distinction matters.** **UDAM** and **Ocean Enterprise** are **marketplace infrastructure**—they enable buying and selling data but don't include datasets. **Company Atlas** is a **data product**—it aggregates firmographic records but has no marketplace or licensing. **PortalJS** and **Data Fair** are **data portals**—they publish and visualize datasets (typically open data), not monetize external data. **None of these are a full DaaS replacement for ZoomInfo or Clearbit.**

- **True open-source DaaS is essentially nonexistent.** No mature open-source project matches ZoomInfo, Clearbit, People Data Labs, or Snowflake Data Marketplace in scope (pre-packaged datasets, enrichment APIs, licensing, compliance). **UDAM** is the closest for marketplace infrastructure, but you must supply the data services. **Ocean Enterprise** is the most sophisticated for privacy-preserving data monetization, but its blockchain architecture is a significant barrier to mainstream adoption. **Organizations needing ready-to-use external data will require SaaS.**

- **Ocean Enterprise's Compute-to-Data is genuinely differentiated.** It enables selling access to private data without transferring the data itself—only computation results leave the premises . **This is relevant for healthcare, financial services, and any organization with data that cannot be moved.** The trade-off is blockchain complexity and crypto wallet management.

- **UDAM is early-stage but functional.** It provides Stripe payments, encrypted token issuance, and concurrency-safe order processing out of the box . **However, it is a backend infrastructure project**—expect to build the frontend, data service integrations, and listing management on top.

- **Pricing opacity is universal across commercial DaaS vendors.** Snowflake, Databricks, ZoomInfo, Clearbit, People Data Labs, Enigma, Coresignal, Crunchbase, Experian, and Workday all require sales contact or usage-based estimation for quotes. **Validate with direct vendor conversations against your actual data volume and enrichment needs.**

- Self-hosted open-source solutions require proper server setup, backup configuration, and ongoing maintenance. **External data and licensing terms are legally sensitive**—ensure your hosting and data handling meet your organization's compliance requirements before deploying.



---



**Made for developers, data teams, and organizations building transparent data-as-a-service solutions.**

Let's make Data-as-a-Service more open, privacy-preserving, and data-provider-friendly.
