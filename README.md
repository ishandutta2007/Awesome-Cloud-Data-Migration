# Awesome-Cloud-Data-Migration

# Awesome-Cloud-Data-Migration

**Top Cloud Data Migration (Opensource) 🌟 Star if you like it! 🌟**



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on ELT/ETL Pipelines, CDC Replication, Connector Ecosystems & Self-Hosted Data Movement*

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud Data Migration**. These tools enable organizations to move data from databases, SaaS applications, and files into warehouses, lakes, and AI applications—from fully managed platforms with hundreds of pre-built connectors to open-source frameworks that give teams complete control over their data pipelines and transformation logic.



**Examples** include Fivetran, Airbyte, Talend, AWS DMS, Azure Data Factory, Informatica Cloud, Qlik Replicate, Matillion, Stitch, and Atlassian Cloud Migration Assistant (the category leaders in commercial space).



**Open-source emphasis**: This section is expanded with every relevant project for self-hosted data integration, ELT pipelines, and open connector infrastructure. **Critical note**: The open-source data movement landscape is exceptionally strong—**Airbyte** is the leading open-source ELT platform with 600+ connectors , **Apache SeaTunnel** handles massive-scale batch and CDC synchronization , and **dlt** represents the modern library-first approach . No open-source project matches Fivetran's fully managed reliability or Talend's enterprise transformation depth out of the box, but for teams willing to operate infrastructure, the open-source options are production-proven at scale.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global data integration and cloud data migration market is estimated at approximately **$15B–$20B** (with the broader cloud migration services market projected to reach **$200B+** by the early 2030s, growing at a ~23–25% CAGR). The market exhibits **moderate fragmentation**: while foundational cloud infrastructure and native migration utilities are concentrated among hyperscalers (Amazon AWS, Microsoft Azure, Google Cloud), the application-level data integration, ELT, and iPaaS ecosystem remains highly dynamic and competitive, populated by independent specialist vendors and open-source platforms to address complex multi-cloud and hybrid environments.

## SaaS/Hosted Platforms

| Platform | Company Size (Valuation / Revenue) | Pricing (Starting Tier) | Free Tier / Trial Limits | Description & Best For |
| :--- | :--- | :--- | :--- | :--- |
| **[Azure Data Factory](https://azure.microsoft.com/en-us/products/data-factory)** | **Microsoft**: ~$3.9T Market Cap / ~$331.8B Rev | Pay-as-you-go: ~$1.00 per 1,000 cloud activity runs; ~$0.25 per DIU-hour for data movement | **First 5 low-frequency activities/month free** (running <= 1/day); 30-day $200 Azure trial credits | Fully managed cloud data integration service with 90+ connectors and visual pipeline design. Best for Microsoft Azure-native environments. |
| **[AWS Database Migration Service (DMS)](https://aws.amazon.com/dms/)** | **Amazon (AWS)**: ~$2.6T Market Cap / ~$717B Rev | Provisioned: `dms.t3.micro` from ~$0.018/hr; Serverless from ~$0.082 per DCU-hour | **750 hours/month** of Single-AZ `dms.t3.micro` + 50 GB storage free for 12 months on AWS Free Tier | Managed database migration and ongoing CDC replication into RDS, Aurora, and Redshift. Best for AWS-centric workloads. |
| **[Atlassian Cloud Migration Assistant](https://www.atlassian.com/)** | **Atlassian**: ~$57B Market Cap / ~$6.57B Rev | Migration tool is **Free**; Atlassian Cloud Standard starts at ~$7.75/user/month (Jira) | **Free forever plan up to 10 users & 2 GB storage** per product (or matching-duration Cloud Migration Trial) | Specialized native migration tooling (JCMA, CCMA) for transitioning Jira/Confluence Server or Data Center workloads to Atlassian Cloud. |
| **[Qlik Replicate](https://www.qlik.com/)** | **Qlik**: ~$10B Valuation / ~$750M–$1B Rev | Enterprise contracts start at ~$1,000/month (quote-based per endpoint/volume) | **No self-service free tier or trial** (custom sales PoC and guided demo upon request) | High-throughput enterprise Change Data Capture (CDC) and streaming replication supporting mainframe, SAP, and legacy enterprise databases. |
| **[Informatica Cloud (IDMC)](https://www.informatica.com/)** | **Informatica**: ~$7.6B Market Cap / ~$1.6B Rev | Usage-based via IPUs (Informatica Processing Units) starting ~$90–$100/IPU/month; entry contracts ~$50K/year | **25 IPUs/month free** on Cloud Data Integration Free Service; or **30-day free trial** with access to IDMC modules | Enterprise-grade iPaaS offering comprehensive data cataloging, governance, mass ingestion, and ETL/ELT pipelines for complex enterprise environments. |
| **[Fivetran](https://www.fivetran.com/)** | **Fivetran**: ~$5.6B Valuation / ~$300M+ ARR | Standard plan starts at ~$500 per million Monthly Active Rows (MAR) + $5/connection base | **500,000 MAR/month free forever** (+ 3,500 reverse ETL rows & 5,000 dbt runs); 14-day free trial with unlimited MAR | Automated zero-maintenance ELT pipeline with 700+ connectors and schema drift management into modern cloud warehouses. |
| **[Talend (Qlik Talend Cloud)](https://www.talend.com/)** | **Qlik / Talend**: ~$2.4B Acq. / ~$350M Rev | Starter tiers start at ~$300/month (billed annually); full enterprise packages scale from ~$50K+/year | **14-day free trial** with pipeline capacity testing limits (Talend Open Studio retired) | Heavy-duty enterprise data integration, API services, and data quality/governance engine. |
| **[Airbyte Cloud](https://airbyte.com/)** | **Airbyte**: ~$1.5B Valuation | Standard tier starts at base ~$10–$20/month; usage at ~$2.50–$5.00 per credit (Open-source self-hosted is free) | **14-day free trial** including **400 free trial credits** (~100 GB data transfer, no credit card required) | Managed version of the leading open-source ELT platform with 600+ pre-built connectors and no-code Connector Builder. |
| **[Matillion](https://www.matillion.com/)** | **Matillion**: ~$1.5B Valuation / ~$100M ARR | Consumption-based starting at ~$2.00–$3.50 per credit (Teams tier starts at ~$1,000/month) | **14-day free trial** including **500 free credits** for 1 developer user (Developer tier) | Cloud-native pushdown ELT/ETL platform running transformation compute directly inside Snowflake, Databricks, Redshift, and BigQuery. |
| **[Stitch](https://www.stitchdata.com/)** | **Qlik / Talend**: ~$60M Acq. by Talend | Standard plan starts at **$100/month** for 5 million monthly rows (scales up with volume) | **14-day free trial** with **unlimited row replication** (no credit card required) | Developer-friendly, lightweight ELT data pipeline tool focused on fast, straightforward ingestion from SaaS and database sources. |



## Open-Source GitHub Projects



- **[Airbyte](https://github.com/airbytehq/airbyte)**

  **Open-source data integration platform for ELT pipelines** (license per repo, ~20K+ stars) — **the leading open-source alternative to Fivetran and Stitch**, with the largest connector ecosystem in open source . **Features**: **600+ connectors** for APIs, databases, data warehouses, data lakes, and AI applications; **Connector Builder** (no-code) and **CDK** (low-code) for creating custom connectors; **Airbyte Agents** and open-source **Agent SDK** (`uv pip install airbyte-agent-sdk`) for giving AI agents real-time access to business data, working with pydantic-ai, LangChain, OpenAI Agents, and FastMCP ; orchestration via Airflow, Dagster, Kestra, or the Airbyte API . **Tech stack**: Java (platform), Python (connectors). **Deploy**: Self-hosted (Docker, Kubernetes) or Airbyte Cloud. **Trade-off**: **Operational overhead**—self-hosted Airbyte requires maintenance for platform and connectors. Connector quality varies; some community connectors are less robust than commercial alternatives. **Best for**: teams wanting a proven open-source ELT platform with the broadest connector coverage and an active community—especially those moving data from SaaS apps into warehouses without per-row SaaS costs.



- **[Apache SeaTunnel](https://github.com/apache/seatunnel)**

  **Distributed, high-performance data integration platform** (Apache 2.0, ~8K+ stars) — **the strongest open-source option for massive-scale batch and CDC synchronization**, trusted by Weibo, Tencent Cloud, Sina, Sogou, and Yonghui Superstores . **Features**: **100+ connectors** with ongoing expansion; **batch-stream integration**—same connectors for offline and real-time; **CDC support** for MySQL, PostgreSQL, Oracle, SQL Server, MongoDB, and more; **distributed snapshot algorithm** for data consistency; **multi-engine support** (SeaTunnel Zeta Engine, Flink, Spark); **JDBC multiplexing** for efficient multi-table sync; high throughput with low latency; **real-time monitoring**; **SeaTunnel Web** for visual job management . **Tech stack**: Java. **Deploy**: Self-hosted (SeaTunnel Zeta, Flink, or Spark). **Trade-off**: **Steeper operational learning curve than Airbyte**—requires understanding of engine selection and job configuration. Smaller connector ecosystem than Airbyte. **Best for**: organizations needing high-performance, large-scale data synchronization (batch and CDC) with multi-engine flexibility—especially those already running Flink or Spark infrastructure.



- **[dlt (data load tool)](https://github.com/dlt-hub/dlt)**

  **Library-first data loading framework in Python** (Apache 2.0) — **the most modern, developer-friendly approach to data pipelines**, designed to be `pip install`ed into existing code rather than operated as a platform . **Features**: **Declarative REST API sources**; **SQL database reflection**; **file sources** (CSV, JSONL, Parquet from S3, GCS, Azure); **DataFrame/Arrow support**; **20+ destinations** by swapping a destination string (DuckDB, Snowflake, BigQuery, Redshift, Postgres, Iceberg, Delta, filesystem) ; **automatic schema inference, DDL generation, and schema drift handling**; **incremental loading and merge strategies via decorators**; **built for LLM and coding agents**—designed from the ground up for prompt-to-pipeline workflows . **Tech stack**: Python. **Deploy**: Embedded in your Python application (`pip install dlt`). **Trade-off**: **Library, not a platform**—you own orchestration, scheduling, and monitoring. No GUI or connector marketplace. **Best for**: Python developers and data engineers who want clean, testable, version-controlled pipelines in their existing codebase—without adopting a heavyweight platform or SaaS subscription.



- **[Apache NiFi](https://github.com/apache/nifi)**

  **Easy-to-use, powerful, and reliable system to process and distribute data** (Apache 2.0, ~5K+ stars) — **the most mature open-source dataflow automation tool**, with a browser-based UI for designing and monitoring pipelines . **Features**: **Browser UI** for design, control, and monitoring with runtime management and versioned pipelines; **provenance tracking**—searchable history with graph data lineage from source to destination; **guaranteed delivery** with retry and backoff; **horizontal scaling** with clustering; **extensible processors** (native Python support); **secure by default** with HTTPS, OIDC/SAML SSO, and role-based access . **Tech stack**: Java. **Deploy**: Self-hosted (Java 21 required). **Trade-off**: **Heavier than library-first tools**—requires Java runtime and operational management. Not a simple ELT tool; better suited for complex dataflow orchestration. **Best for**: organizations needing a proven, secure dataflow platform with visual design, provenance, and clustering—especially those handling sensitive data with compliance requirements.



- **[Meltano](https://github.com/meltano/meltano)**

  **Open-source, convention-based data platform** (MIT) — **the "GitLab of data" approach**, bringing version control and CI/CD to ELT pipelines . **Features**: **Singer-based ELT**—extractors, loaders, and transformers managed via YAML; **CLI-driven workflow**—pipelines defined in code, versioned in Git; **dbt integration** for transformations; **500+ Singer taps and targets** available; **state management** with S3/GCS/Azure backends . **Tech stack**: Python. **Deploy**: Self-hosted (`pip install meltano`). **Trade-off**: **Singer ecosystem is less active** than Airbyte's; fewer connectors and slower updates. CLI-only; no GUI. **Best for**: teams wanting a convention-driven, Git-native ELT workflow with strong dbt integration—especially those already invested in the Singer ecosystem.



### Additional Strong Open-Source Options



- **Talend Open Studio** — Free, open-source version of Talend's ETL tool (Apache 2.0). **Note**: The open-source edition is **in maintenance mode**; Talend's commercial platform is the actively developed product. **Best for**: teams with existing Talend Open Studio jobs, not new greenfield deployments .

- **Fivetran Connector SDK** — Open-source SDK for building Fivetran connectors (MIT). Community connectors available on GitHub. **Note**: **SDK for Fivetran's managed platform**, not a standalone data movement tool—connectors run on Fivetran's infrastructure . **Best for**: teams already on Fivetran wanting to build custom connectors for niche sources.



**Frameworks for building custom systems**: Combine **Airbyte** as the broad connector platform with **SeaTunnel** for high-volume batch and CDC synchronization, **dlt** for Python-native pipelines where you want code-level control, and **NiFi** for complex dataflow orchestration with provenance—creating a data migration stack matched to each team's scale and technical preferences. **None of these match Fivetran's fully managed reliability or Talend's transformation depth**, but for teams willing to operate infrastructure, the open-source options cover virtually every data movement need.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Cloud data migration platforms handling production data must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate encryption, access controls, and audit logging during migration.

- **The "managed ELT platform" vs. "high-performance integration engine" vs. "library-first framework" vs. "dataflow automation" distinction is critical.** **Fivetran, Airbyte Cloud, Talend, AWS DMS, Azure Data Factory, Informatica Cloud, Qlik Replicate, Matillion, and Stitch** are **managed platforms**—they provide hosted infrastructure, scheduling, and monitoring. **Airbyte (self-hosted), SeaTunnel, and Meltano** are **self-hosted platforms**—you own the infrastructure and operations. **dlt** is a **library**—it embeds in your code; you own orchestration. **NiFi** is **dataflow automation**—it handles complex routing and transformation, not simple ELT. **Choose based on whether you want managed convenience, platform control, code-level flexibility, or complex dataflow orchestration.**

- **Airbyte is the pragmatic default for broad connector coverage.** 600+ connectors, an active community, and a Connector Builder make it the closest open-source analog to Fivetran—without per-row costs . **The trade-off**: self-hosted operations and variable connector quality.

- **SeaTunnel is the choice for massive-scale batch and CDC synchronization.** Trusted by Weibo and Tencent Cloud, with a distributed snapshot algorithm for consistency and multi-engine support (Zeta, Flink, Spark) . **The trade-off**: steeper learning curve and smaller connector ecosystem than Airbyte.

- **dlt represents the future of developer-first pipelines.** It is a library, not a platform—`pip install dlt`, write Python, and load to 20+ destinations with automatic schema handling . **For teams frustrated by platform lock-in and YAML-heavy configuration, dlt is the cleanest path to maintainable pipelines.**

- **Talend Open Studio is in maintenance mode.** The open-source edition has not received significant updates; Talend's commercial platform is the actively developed product . **Do not start new projects on Talend Open Studio** unless you have existing investment.

- **Pricing opacity varies.** Fivetran, Airbyte Cloud, AWS DMS, Azure Data Factory, Matillion, and Stitch publish consumption-based pricing. Talend, Informatica, and Qlik Replicate require sales contact. **Validate with direct vendor conversations against your actual data volume and connector requirements.**

- Self-hosted open-source solutions require proper infrastructure (servers, databases for state, orchestration tooling), security hardening, and ongoing maintenance. **Data migration pipelines handle production data**—ensure your deployment includes monitoring for pipeline failures, schema drift handling, and data quality validation before relying on it for business-critical analytics.



---



**Made for data engineers, analytics teams, and organizations building transparent cloud data migration solutions.**

Let's make Cloud Data Migration more open, data-driven, and pipeline-reliable.
