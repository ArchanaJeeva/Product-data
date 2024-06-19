**IBM watsonx.data (lakehouse) INTERNAL to IBM (Confidential) FAQ for Seismic**

Updated Apr 12, 2024

**For the most up to date information about watsonx overall visit the watsonx saleskit on seismic <https://ibm.biz/watsonx-saleskit>**

## **Frequently Asked Questions (FAQ) about IBM watsonx.data (a fit-for- purpose data store built on an open lakehouse architecture)**

**For the most up to date information about watsonx.data you can refer to** 

- **watsonx.data saleskit on seismic [https://ibm.biz/watsonx-data-saleskit**](https://ibm.biz/watsonx-data-saleskit)**
- **Documentation [for customer-managed environments](https://www.ibm.com/docs/en/watsonxdata)** 
- **Documentation for [fully managed SaaS**](https://cloud.ibm.com/docs/watsonxdata)**
##
## **Product:**
What is a data lakehouse? 

A data lakehouse combines the best features of a data lake and a data warehouse. At its core it enables a customer to

1. Store: Leverage object storage – for disruptively affordable data storage 
1. Format: Open data and table formats to allow interoperability and
1. Query: open source query engines to query and make sense of the data on demand
1. Governance: share data with who needs it and has permissions, and not with everyone 

Why did we choose the technologies we did as the foundation of watsonx.data (IBM’s open data lakehouse which we will sometimes refer to as “lakehouse” in this FAQ)? 

1. Storage: S3 API based  object storage is a de facto storage standard for affordable storage. 
   1. Public Cloud: based on deployment, AWS S3 or IBM Cloud Object Storage/CoS) can provide the cloud-scale storage for watsonx.data  at an affordable cost with control over the data
   1. On-premises: IBM Storage Ceph can provide an open, scalable and software defined object storage. It is engineered with resiliency so there is no single point of failure, a critical differentiator as IBM Storage Ceph is optimized for enterprise data storage at petabyte-scale. 
1. Open Data and Table Formats:
   1. Table: Iceberg is the open table format with market leading adoption. It brings ACID transaction support,  massive scale and speed and critically, upon our architects careful review of the market and comparisons (e.g. to Delta Lake and HUDI) it became clear this is the direction the market and community is embracing first, so we will too!
   1. Data formats: Parquet and ORC are the most common and adopted open formats
1. Query: Multi engine- there is NO one engine to rule them all, so IBM will be first to market with multi-engine lakehouse support built in!
   1. Presto (Ahana-enhanced) for BI purposes, SQL and dozens of connectors – allows for speed and efficiency - this was also chosen upon our architects careful review of the market and comparisons (e.g. Trino) as a ***more open*** open-source engine with a promising future and an exciting roadmap we can collaborate on
   1. Spark: for AI/ML workloads to make unstructured data from the data lake useful
   1. IBM Data Warehouse engines: run the highly tuned IBM DW engines on your IBM Data warehouse for the best tuning and high speed responses when needed
1. Governance: 
   1. Built in: the basics of Role Based Access Control (RBAC) and 
   1. Watson Knowledge Catalog (WKC): highly customize able and powerful governance through our integration with WKC (sold separately) 
1. Hybrid Cloud /private cloud / on premises / on-prem software deployments
   1. SaaS on AWS and IBM Cloud 
   1. On-prem or customer managed environment on OpenShift Container Platform (OCP) as a cartridge on Cloud Pak for Data CP4D) 

What is core value prop messaging we all should be using, or is it just "cost optimization"?

1. Cost optimization: save 50% of costs by choosing the right engine for the right workload and dynamically pausing/resuming engines
1. Return on data: by enabling customers to get easy access to all their data – existing and new and across hybrid cloud environments, and leveraging cost-efficient object storage.
1. Faster time to value: by reducing data movement and ETL, data onboarding and pipelining lead times, built-in security and governance through integration with data fabric 

What are key functionalities we should be showing customers?

1. Demonstrate Db2 Warehouse & Netezza workload offloading for customers modernizing their on-prem warehouse appliances to SaaS
1. Demonstrate data sharing between different engines for customers looking to enhance data lake analytics and achieve broader workload coverage

What is expected in GA? 

1. The ability to quickly get started and start analyzing data
1. The ability to share/bring an S3 object storage bucket
1. The ability to query these with the Presto engine 
1. The ability to create/start/stop multiple Presto engines
1. The ability to query these with the IBM Spark engine by connecting to an external spark engine (e.g. IBM Analytics Engine or Apache Spark on Amazon EMR) – with full inclusion of Spark internal to watsonx.data in a future release
1. The integration points (connectors) between Netezza and Db2 Warehouse in SaaS
1. Metadata synch between watsonx.data and Db2 Warehouse and Netezza 
1. Caching powered by Raptor X
1. Deploy SaaS on AWS or IBM Cloud 
1. Deploy software on-prem on OCP standalone or with CP4D

Does watsonx.data include licensing to use CP4D? OCP? Does it require them?

- Yes, as a cartridge on CP4D watsonx.data requires using both CP4D and OCP underneath the install and includes limited licensing to each specifically to deploy and use watsonx.data only. Separate entitlements to CP4D can be purchased to deploy and use other value added CP4D services alongside that work well with watsonx.data like Watson Knowledge Catalog (WKC) or IBM Analytics Engine (based on Apache Spark) 

How do we understand the visionary demonstrations (like at THINK) the indicate product direction vs what is in the product at GA or other given times?

1. Our demos at think are intended to show what will be available in the product by end of year there are generally 3 levels of feature access
   1. Private Preview: special arrangements for select customers to access features 
   1. Open preview: available to try to any customer but not supported at production level
   1. Generally Available: GA fully supported and available to all to buy
1. We will use our roadmap on seismic to identify major items demonstrated at THINK that are not yet available in GA and when they are targeted for in our Continuous Delivery (CD) release cadence 
1. All of these features and timings should be considered directional as per IBM disclosures, disclaimers and NDAs

Which regions will SaaS be hosted in at GA?

1. The most current SaaS regions are displayed in the IBM cloud catalog launch and provisioning page 
1. Location
   1. Dallas
   1. Washington DC
   1. Frankfurt
   1. London
   1. Tokyo
   1. Northern Virginia
   1. Oregon


Guides for specific use cases so we can prove value props like “optimization” to customers

- High level use cases we have identified: 
1. Streamline business processes: Eliminate duplication and simplify your business' use of warehouse and lakehouse data using a single point of entry built on object storage and shared metadata. 
1. Real-time insights across all your data: Speed time to insight and power your analytics and AI with fresh data from all types of data sources without the need to access multiple systems or move and copy data. 
1. Share data responsibly: Easily share and work with your latest data in a responsible way using a open and governed data repository.
1. Accelerate AI adoption: Build and train trusted AI/ML models across all governed data leveraging multiple languages and query engines inside the lakehouse and utilize semantic automation to clean, connect, and enrich lakehouse data for AI.
- On optimization of price performance very specifically: On an apples-to-apples basis, IBM watsonx.data Presto VPC/hr is 50-20% less expensive than Snowflake and Databricks, so running any supported workload on IBM watsonx.data Presto will help customers reduce cost.  Most likely, the low-hanging fruit are data transformation ELT, big-data scans/joins, and ml model training workloads that can be offloaded from a data warehouse to a lakehouse engine and achieve acceptable performance at lower costs.  BI-like queries of historical data that are not subject to strict sub-second SLAs are also candidates for shifting to the lakehouse.  More details on workload assessment and optimization step-by-step to follow.
- We have early manual tooling to optimize workloads with warehouse offload identification and are working to automate and build out mor rapid analysis of workloads that might be better suited for use in the watsonx.data. 

Can you list scenarios and use cases where client will be interested by on-premises lakehouse as most factors like cost saving might not be significant on-premises ?

1. For on-prem scenarios, it's not only about costs, it's also regulations and a need to keep data on-prem. IBM is one of the few vendors (only vendor?) who can provide a true hybrid cloud story in the lakehouse space today
1. Modernization is important, irrespective of on-prem or cloud. The reality is every client wants off Hadoop. Today, the leading option has been Databricks - who only exists on cloud. Many clients have PBs of data in their on premise data lake, and are unwilling to migrate that to cloud. Our lakehouse is designed to augment or modernize existing data lakes. We can simply point lakehouse to an existing Hadoop cluster and start querying right away.

Does the watsonx.data lakehouse offer a connector for Cloudera?

1. Hive access will be available at GA. 
1. HDFS support is in progress but will not land at GA. 
1. Impala access is not currently in roadmap.
1. HBase access is not currently in roadmap.

What is the migration effort required by on-premise Db2 Warehouse, NPS and Cloudera (Hive) deployment to watsonx.data ?

- The idea is not to migrate data. Since the GA of watsonx.data, Db2WH and Netezza now also support Hive Metastore, Iceberg Table format and storage on S3 object storage formats

Will our Iceberg format offer full Insert/Update/Deleting Rows? Will data actually get deleted, or just marked obsolete ?

- Iceberg does support both Update and Delete concept via a Merge on Read paradigm. You can read more in the Iceberg open source documentation 
  <https://iceberg.apache.org/docs/latest/spark-writes/>

How do I perform SQL DDL or DML on an Iceberg Table?	

- Iceberg is not a query engine and thus does not have any SQL functionality by itself. To perform DML or DDL operations on Iceberg data you need to use a supporting query engine like Presto or Spark which support them.

Databricks use Deltalake format, will we support this either in watsonx.data or with Db2 WH/Netezza?

- ` `Deltalake is being considered for the longer-term roadmap. Even though they have claimed open source, Delta Lake is decidedly “closed governance” it is still a project dominated by Databricks and there have been issues getting changes into projects owned by Databricks, Spark as an example.

Is there a plan to support other tables formats or catalogs? Why did we choose Iceberg?

- Possibly. There are 2 other popular open table formats today: Delta Lake and Apache Hudi:  with Delta Lake, although it is claimed to be Opensource, it is very “closed governance” Databricks control a lot of it. Another Table format that was considered by development was Apache Hudi which might become supported down the line depending on its usage by the community.
- Others being considered include informatica catalogs, Azure ADLS Gen 2 and others being considered in accordance with market demand

How will watsonx.data integrate with Identity and Access Management (IAM) solutions?

- When deployed on SaaS IBM Cloud IAM will be integrated. 
- When deployed in software there are plans for integrations to underlying identity providers – with the option of more advanced data governance from Watson Knowledge Catalog (bought separately in CP4D) for customers that need it. 

The UI looks great but what if a customer wants to work in their own separate enterprise environment for SQL? How can a customer work with watsonx.data without using the AI? Can they access by CLI by API? 

- Yes, they can connect to watsonx.data by JDBC to the engine. 
- That way you can use your own SQL tool or IDE. 

How should customers do ETL along with watsonx.data – should they use DataStage? 

- We think often they can use spark to do transformations of the data – they can use spark to define a data frame and transform the data sitting in object store in the watsonx.data lakehouse. Because of ability to work at file and table level. 
- Taking files and doing transformations before landing data is possible using presto CLI and ingest tool native in the product. 
- For those already using Db2 or Netezza for warehousing, theose data warehouse can write to Iceberg and thus share their data with watsonx.data and vice versa. 
- Those that have existing ETL, could start landing data into object storage, then they could transform to Icberg table forms
- Datastage is working on adding Iceberg as a format they can write to as well as a part of their roadmap. 

What about unstructured data formats?

- We’re starting first with focusing on open data and table formats (Parquet, ORC, Avro)
- We are also considering additional data formats for prioritization in our roadmap, please share feedback from customers about what additional formats are most demanded and valuable!

**Sales Support,  Tech Sales Coverage:**

Mechanism for engaging with PM for customer feedback/support?

- We began watsonx.data office hours in April, and currently plan to continue 2x monthly deal assistance office hours. The [series will be linked here on seismic.](https://ibm.seismic.com/Link/Content/DCgQX688HgqFXGTDWdWMdc9jhWqj) 
- There is an open slack channel in which all IBMers can share their feedback 
  - #ibm-watsonx-data-lakehouse-feedback
  - [Link](https://ibm-analytics.slack.com/archives/C04TPNQUEP8)

What is plan for technical SWAT team to ensure great coverage for each account?

The watsonx.data Tech Sales Activation Team can provide assistance based on prioritization through tech sellers and Global Sales leadership.  

- For more details visit the tech sales activation [publisher page](https://ibm.biz/watsonx-data-tech-sales) 

How will leads be captured, tracked/managed, qualified?

- Pipeline opportunities [are tracked in ISC per these instructions](https://ibm.seismic.com/Link/Content/DCQjRFTDgmT7f8hV7h2XqBMdXcj3) 
- ISC opportunities must be created for prioritization through Global sales for any additional support needed for deals.

What is the plan for ongoing enablement? 

- [Stay tuned to seismic and enablement channels](https://ibm.seismic.com/Link/Content/DCgQX688HgqFXGTDWdWMdc9jhWqj) for updates on the many opportunities were planning for enablement!

Can we expect any help from AWS for our efforts?

- AWS actively engaged largely via PM and engineering. 

What is the level of technical sales readiness?

- The Technical Sales watsonx.data (lakehouse) Activation Team, led by Bradley Rowen, is a group of selected IBMers from Tech Sales who have led the training and enablement for tech sellers. This group will be available as client advocates as prioritized by tech sales and Global sales leadership and will assist in scaling education to the remaining members of the HDM sales and technical sales community. Their [publisher page is here.](https://ibm.biz/watsonx-data-saleskit)

What is best practice for capturing opportunities in ISC?

- Detailed instructions can be found [here on seismic](https://ibm.seismic.com/Link/Content/DCQjRFTDgmT7f8hV7h2XqBMdXcj3)  
##
## **Selling, pricing, competing:**
Demonstrations and Trials 

- Leverage Techzone for demonstrations  <https://ibm.biz/wxd-techzone>
- Customers may self-serve access a lite plan for free (**coming soon! (tgt before THINK)** [to try watsonx.data in IBM Cloud](http://cloud.ibm.com/watsonxdata) for a limited period of time and resources. 

What are the pricing plans for fully managed SaaS? 

**Lite plan (tgt before THINK):** The Lite plan is provided for you to try the basic features of watsonx.data and is available to all IBM Cloud account types like trial, pay-as-you-go, and subscription. It supports the basic features only. It is not available on AWS and is limited to one watsonx.data instance per IBM Cloud account (cross-regional).

**Enterprise plan GA:** You must have a pay-as-you-go or subscription IBM Cloud account to avail the Enterprise plan. It is available on IBM Cloud and AWS environments. Presto engine and Milvus service are available with this plan.

**Enterprise with BYOL (Bring Your Own License): coming soon! (tgt before THINK)** With this plan, you have everything from the [Enterprise plan](https://test.cloud.ibm.com/docs-draft/watsonxdata?topic=watsonxdata-pricing-plans-1#enterprise-plan) in addition to a discount on IBM-managed SaaS by allocating your previously purchased self-managed environment (on-premises) perpetual or subscription licenses.

<a name="_toc1491135583"></a>**More on Lite Plan:**

Is the lite plan credit card free?

- A. Yes, by using an IBM cloud trial account the lite plan is credit card free. You have a set amount of free usage limit of 2000 Resource Units within a timeframe of 30 days, whichever ends first,  to try the product. For more information, see the lite plan tutorial in the IBM cloud SaaS docs

What's included in the lite plan?

- The lite plan includes the following features and limitations:
  - It enables provisioning of a single lite plan instance per resource group.
  - It provides a free usage limit of 2000 Resource Units (monitored on the Billing and usage page of IBM Cloud) within a timeframe of 30 days. The cap value is displayed on the IBM Cloud catalog provisioning page and is reflected on your billing page within your watsonx.data instance upon provisioning.
  - With the lite plan instance, you can create either one starter Presto or one starter size Milvus service, or both.
  - The Quick start path is simplified in lite plan. For more information, see Getting started.
  - Ability to pause and resume Presto engine.
  - Ability to connect to an IBM Cloud-provided Cloud Object Storage (COS) bucket and provide credentials to your own COS or S3 bucket.
  - Ability to delete Presto, Milvus, and connections to your own bucket.
  - The Billing and usage facilitates monitoring of resource usage through IBM cloud.
  - The lite plan is limited to a maximum of one Presto engine or Milvus service or both.
  - The lite plan is limited to the smallest node sizes and profiles for each engine and service. You cannot increase the node size.

What is the limit for using the lite plan?

- A. The lite plan of IBM® watsonx.data instance is typically a trial account that is free to use, with limits on capacity (2000 Resource Units), features for a time frame of 30 days. You can use the account to explore and familiarize yourself with watsonx.data. You need to convert your lite plan to a standard plan instance to access all the features and functionalities.

I have exhausted all my resource units - How do I delete my lite plan instance?

- A.  You can delete the lite plan instance from the resource group or IBM cloud resource collection removes it after a period of 40 days.

The lite plan has ended—how do I upgrade to the enterprise plan?

- Once your lite plan has concluded, you can purchase the “Subscription“ or “Pay as you go“ enterprise plan on IBM Cloud when creating your new watsonx.data instance. The enterprise plan is available on IBM Cloud and AWS environments.

What is the pricing for all of watsonx.data? 

- Pricing information can be found on the seismic saleskit.  <https://ibm.biz/watsonx-data-saleskit>

What is recommended sizing? 

- T Shirt sizing is available on seismic saleskit. https://ibm.biz/watsonx-data-saleskit
- A sizing estimation calculator for SaaS [is built into the IBM cloud console](https://test.cloud.ibm.com/lakehouse) in the “About” section before service creation 
- Sizing information for watsonx.data is also built into the [Cloud Pak for Data configurator](https://app.ibmsalesconfigurator.com/#/zen/configure). 

![](Aspose.Words.e1c061b4-a900-4a7c-9fcc-0ac59b34a89e.001.png)

Understanding of how we position to work with Databricks?  When and how to compete?

**IBM’s will be the only data lake that offers multi-engine support.**

Databricks **is pure compete**, co-exist really doesn’t make sense at this point in time

1. We will compete on the workload coverage aspect with our multi-engine approach where Databricks only has Spark
1. Generally, Databricks is a “walled-garden” and SaaS-only lakehouse and we will differentiate on price/performance, openness/interoperability and hybrid-cloud deployment models.
1. openness/interoperability since we will support Iceberg vs. DeltaLake (Databricks standard – less openly and cooperatively maintained) for open table formats.
1. Sales competitive decks and “battlecards” will help with this - <https://ibm.biz/watsonx-data-saleskit>

Same question for Snowflake?

**IBM’s will be the only data lake that offers multi-engine support.**

1. IBM watsonx.data **will be able to co-exist** with Snowflake through warehouse optimization via connectivity and Iceberg support.  Certain workloads/data will remain on Snowflake, while others will be offloaded to Lakehouse
1. Generally, Snowflake is a monolithic and proprietary SaaS-only data warehouse and we will differentiate on price/performance, openness/interoperability and hybrid-cloud deployment models.
1. Sales competitive decks and “battlecards” will help with this <https://ibm.biz/watsonx-data-saleskit>

What is vision/roadmap for Product vs what’s available now? 

1. Our sales enablement and demos are intended to show what will be available in the product by end of year 
1. We will use our roadmap on seismic to identify major items demonstrated at THINK that are not yet available and when they are targeted for in our CD release cadence 
1. All of these should be considered directional as per IBM disclosures, disclaimers and NDAs

What is our compelling list of uniqueness's? When will each get delivered?

1. Multi-engine. Support for query multiple-engines that provides fit-for-purpose price/performance and functionality for a broad range of workloads 
1. Support for hybrid-cloud deployment models (multi-cloud SaaS and on-prem w/ BYOL)
1. Built-in governance and automation (policy enforcement) with centralized governance with WKC 

Are we adding anything proprietary on top of OS Presto—whether that’s enhancements or ease of deployment, etc?

1. Presto is a query engine, watsonx.data is a complete lakehouse with multi-engine choices
1. A unique UI to simplify deployment and configuration
1. we are leveraging the custom connectors we built (to Db2 and Netezza) and the 
1. improvements Ahana made to the Presto engine
1. Deployment capabilities on CP4D cartridge brings true hybrid capabilities and
1. Saas deployments on AWS or IBM Cloud

Will Presto be enhanced to introduce new features?

- Yes. The objective for IBM is to be a prime contributor to Presto future and be able to influence the roadmap of such product accordingly, taken our client’s needs into account. The acquisition of Ahana will help us accelerate such strategy.
- This will include testing and supporting additional of the open source Presto connectors
- We also plan to leverage the Open Source Prestissimo /Velox projects to substantially improve query speed in Presto you can learn more [here](https://ahana.io/uncategorized/ahana-to-present-about-prestos-query-optimizer-and-the-velox-source-project-at-prestocon/)

Will we get reference architectures for on-premises proposals ?

- Yes, these are in progress.

How could the lakehouse announcement affect Cloudera partnership?

- This should help strengthen our partnership with Cloudera. Cloudera is proposing a very similar message, and also supporting Iceberg.
- We are looking to augment and complement Cloudera with our watsonx.data 
- What that means is that it should be easier to align CP4D with Cloudera now.

Does this compete with a data warehouse directly? Our own. Netezza, Db2 or others, competitors

1. The first and most important emphasis is coexistence and collaboration. Some workloads (high performance SQL queries with specified SLAs etc. really do need to be on warehouses.
1. Older data, transformations, these kinds of workloads might be better handled at better price-performance by a lakehouse – search this FAQ for “workload” to read more about this
1. Some competition may occur over time as customers compare their needs and uses between a lakehouse and a cloud data warehouse.
1. A strong method of comparison is to consider the “medallion” architecture or “gold, silver bronze” concept, in which “gold” refers to high performance DW queries, “silver” to those that can tolerate a bit more time at lower cost and “bronze” is for exceedingly high volune less structured data. 

What possible ways do we feel Netezza Db2 warehouse, CP4D and other products may be more easily positioned and sold if a customer buys into watsonx.data? What are the cross sell opportunities?

- If you have Netezza or Db2 Warehouse you should add a watsonx.data– it adds new cost optimization and broader/new workload coverage capabilities. 
- Likewise if you buy watsonx.data you should buy a high performant data warehouse that also reads from and writes to Iceberg format, which Db2 and Netezza plan to at the GA of watsonx.data. 
- There is more detailed cross sell deck guidance in the [saleskit on seismic](https://ibm.biz/watsonx-data-saleskit). 

Competitive guidance for positioning watsonx.data for AI workloads as well as Warehouse workloads

**IBM’s will be the only data lake that offers multi-engine support.**

1. Workload supporting AI such as tokenization, encoding, enrichment, data cleanse and prep should all be done in the lakehouse with lakehouse engines.
1. Organized and structured data ready for reports and dashboards should be attempted in the watsonx.data or promoted to the warehouse depending on performance SLAs

Competitive info Dremio, Starburst, Athena (in addition to Databricks/Snowflake from above)? 

If AWS shop today, why not Athena?

1. Sales competitive decks and “battlecards” will help with this – they are available in seismic saleskit <https://ibm.biz/watsonx-data-saleskit>
1. Athena is just a serverless query engine that works with Glue and S3 to form a lakehouse, it is only a part of a lakehouse solution that requires more effort for customers to manage
1. Athena also switched to the Trino distribution which is a fork of Presto largely controlled by Starburst vs Presto’s more open governance model. 
1. Athena also does not provide an on-prem or hybrid deployment option
1. Athena is only on AWS and not other cloud providers
## **Related and Adjacent IBM products:**
Why was Ahana acquired? 

How will Ahana fit with IBM watsonx.data? 

1. Ahana is a major Presto contributor and it will be key within our lakehouse story. 
1. Ahana-enhanced Presto will replace the current community Presto inside watsonx.data. 
1. Ahana as a product will not be resold, and existing Ahana clients will be moved to IBM watsonx.data.
1. Ahana was a tech and people acquisition, they have a great Presto engine and very experienced folks in that space. Further, Ahana gives us credibility with Presto as well as multiple seats on the Presto steering committee.

How will customers use S3 compatible object store on-premises? How will they realize cost advantages if they’re having to build out a local object store?

- IBM recommends Ceph for on premises object storage, which is proven to be performant and economical. Ceph plays the role of the watsonx.data data lake persistent store. 
- IBM watsonx.data software comes with a starter quantity (500 TB usable) of Ceph.
- By partnering with IBM storage, clients can expand the start kit or upgrade to Ceph ready nodes.
- Learn more about how IBM [Storage is integral to watsonx here](https://ibm.seismic.com/Link/Content/DCQDDf46XVgPR8fR8DQXXmb9RVCP).
- We have tested watsonx.data with Ceph, IBM COS, and AWS S3.

Will there be a watsonx.data (appliance) system for on-premises?

- Yes. We are collaborating very closely with the IBM Storage team to deliver the best experience on premises or on the edge with an IBM Storage Fusion HCI appliance. Fusion HCI plays the role of compute and data acceleration for watsonx.data.
- Learn more about how IBM [Storage is integral to watsonx here](https://ibm.seismic.com/Link/Content/DCQDDf46XVgPR8fR8DQXXmb9RVCP).

Will BgSQL be deprecated ?

- BigSQL will not be deprecated in the short term. Once Db2W gen 3 and watsonx.data are stable, this would be considered.

How can customers leverage CP4D VPCs to deploy watsonx.data?

- There is no leverage of CP4D VPCs to watsonx.data entitlements.

If I have a z customer with Db2 for z/OS, what should I do?

- If you have an IBM zSystems customer with Db2 for z/OS you should engage the z seller responsible for the account. 

 

How is Db2 for z/OS data included in lakehouse?

- Db2 for z/OS data can be readily incorporated within the lakehouse via Db2 for z/OS Data Gate for Cloud Pak for Data. Db2 Data Gate provides synchronized Db2 for z/O data to Db2 Warehouse SaaS and software and the lakehouse could readily access this data via the included Presto connectors and the Iceberg table support of Db2 Warehouse.

If Watson Query can see the same S3 data, would we expect watsonx.data to give a faster response ?

- Watson Query does not currently support Iceberg format. Long term support will likely be added but Watson Query supports only a subset of data which can be represented in Parquet/Iceberg formats.

IBM watsonx.data can also virtualize data like Watson Query. Both solutions are integrated with WKC (Business term mapping and Data Masking). What are the positioning WQ vs watsonx.data?

- For a pure virtualization use case, WQ is recommended.
- IBM watsonx.data 's primary role is not for virtualization. Although the connectors allow for that, WQ will be much more efficient and has more advance tech like query rewrite. As of now watsonx.data has nothing like that.
- If the bulk of workloads come through watsonx.data, it would be easier to virtualize from watsonx.data

How should watsonx.data be deployed alongside Cloud Pak for Data? 

- Watsonx.data deploys on a Cloud Pak for Data cartridge. The relationship between CP4D and watsonx.data is that watsonx.data is a data source to CP4D) more [here in docs](https://www.ibm.com/docs/en/watsonxdata/1.1.x?topic=planning-environment-other-cloud-paks)

How will this complement vs compete with SingleStore (or other specific data storage solutions)

- In the future registering engines and pointing them to the consolidated metadata store and iceberg format for persistence and longer term storage, for consolidation and for  governance. And again, workload optimization. 


Bandwidth: how much is being required to be moved by this?

- We aim to move as little data as possible and to minimize duplication. 
- Advanced caching should also help to reduce the need for ground to cloud data movement or need for repeat movements. 




