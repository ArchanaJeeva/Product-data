**Table of Contents (V2)** 

- General discussion points 
- Positioning of watsonx and Cloud Pak for Data Software 
- Packaging and Pricing  
- Product Technical 

**General discussion points** 

**What customers can be migrated from Cloud Pak for Data to watsonx?** 

- There are 2 main sets of customers.  
- First, customers with undeployed Cloud Pak for Data. A fairly easy way for IBM to add value to the undeployed Cloud Pak for Data VPC’s is to make them applicable in support of GenAI and watsonx.  
- Second, deployed or deploying customers that want to standardize on a single GenAI and ML environment. These customers can extend their current Cloud Pak for Data ML environment with GenAI and standardize 

  on a single platform for AI forward with watsonx.  

- Where customers have VPCs deployed for Watson Studio/Watson Machine Learning family services, these should tradeup to watsonx.ai, for Watson OpenScale/FS to watsonx.governance. Note that there is no tradeup path defined for tradeup to watsonx.data.  
- If the customer is deployed, **don't trade up VPCs that are used for other services.** 

**Is there a way to know customer by customer who is eligible and what their current deployment is?** 

- Yes - Target lists of Cloud Pak for Data Base clients (including ELA customers) with Perpetual S&S and Subscription License renewals in 2024 have been provided to the Geo sales leaders. The lists include all renewing customers with their latest deployment information from CSMs indicating whether customers have or have not deployed Cloud Pak for Data Base projects. Customers with no previous deployments are a high priority for the tradeup motion, as are customers who are currently deploying Data Science (Watson Studio and/or Watson Machine Learning services). Other customers in the list are also potential candidates, but must be evaluated for evidence of Data Fabric deployments. Also be cautious when trading up customers indicated to have need for Cloud Pak for Data Base VPCs for future workloads (such as IGC customers trading up to IBM Knowledge Catalog). These data points are all included within the lists.  

**Who should I strategize with then to get the program going?**  

- Understand customer, deployment status, renewal date, and their desire to extend to GenAI and watsonx. LOB and technical owner input will be required to build out a fuller picture of AI business strategy and data management strategy mapped to deployment status. 
- Communicate with and obtain input between Sales, Subscription reps, CSM’s, Tech Sales. Note, there will be varying levels of deployment status for CPD  
- For the subset of ELA accounts who are required to declare the deployment of their entitlements, the Contract Type, CPD Entitled $M, CPD Deployed $M and Lifecycle stage is provided in the Target Lists (see above) for reference.  

**Are there ELA Considerations?** 

- Trade-ups of ELA catalog deployment are only possible when the ELA renews or reopens and the CPD entitlements must be declared (ie there must be a Proof of Entitlement) before they can be traded up.  

**Is the deployment information in the list accurate?** 

- Not always. It’s only accurate if detail is recorded by CSM’s, and the status has not changed since the lists were last refreshed. Therefore a conversation between CSM and Sales is critical to better understand deployment status.  

**Are services available in the migration to help speed deployment?** 

- Yes, TEL planning services for watsonx.ai and watsonx.governance are **mandatory** parts of the program and must be added to bids - and will be checked by L0 approver. Note that Trade-ups have very restrictive discounting so the usual net new strategy of keeping the same envelope price and discounting the SW to free up services $ isn't possible, so budget needs to be built in.  

**What else do i need to do before the sales process can begin?** 

- Work with CSM’s and Tech sales to clearly document the current environment and determine the new as-is CPD and new to-be watsonx environment in the IBM Configurator. 

**When can tradeups and add-ons be offered or transacted?** 

- Approach customers in advance of the renewal time - ASAP for Q2 renewals, but also start now for 2H renewals - especially for undeployed customers.  
- Customers of the perpetual offering can use either the tradeup motion or the Subscription License upgrade motion. Subscription license customers only have the add-on motion.  
- Tradeup provides access to both CPD and watsonx to the total VPC count that they have licensed. CPD VPCs would primarily be used during the transition period - for example the customer would continue to run WML in CPD until such time that they watsonx,ai environment is fully configured. At the end of the transition period, we would expect that all VPCs are running on watsonx.  
- For Subscription license Add-ons, the Add-ons should be co-termed with the CPD environment. At the end of migration customer will renew the watsonx SL license going forward.  

**How do I begin discussion with customers?**   

Are clients fully deployed with CP4D Enterprise Edition**?**   

Or are clients only running ML in current CPD deployment with no Data Fabric plans? Review with customer how Data Fabric fits with Watsonx from capabilities including:  

- Watson Query 
- IBM Knowledge Catalog 

Sales will work with Customer, SE’s, CSM’s to ascertain fit of this program.  2 Items need to be determined, are  

1. Unused VPC’s of CP4D – if so may make sense to transition 
1. Is only ML being used in the CP4D Stack – if so may make sense to transition 
1. What is the size of the to be watsonx environment – Note if doing GenAI now, VPC/VCPU allocations need to account for this.  

**What parts are proposed?   If SL** 

- Watsonx.ai or .gov Add-On contains only watsonx components 
- Mutually exclusive usage of watsonx.ai or watsonx.governance OR from parts 
- At the time of SL renewal, the base license and Add-on convert to a “standard” watsonx.ai or watsonx.governance subscription license 
- Add-On is priced as the difference between the watsonx subscription license and the from part subscription license 

**If Perpetual**  

- watsonx.ai or .governance Transition Edition is a **bundle** of: CP4D Enterprise Edition  and watsonx.ai or .governance 

  *Conversion* Entitlement Ratio of 1 VPC / 1 VPC to CP4D Enterprise Edition OR watsonx.ai 

- The parts exist to simplify customer migration paths and timelines by providing access to both watsonx and CP4D Enterprise Edition  
- The customer would continue with Watsonx.ai or .gov Transition Edition after migration complete 

**Who should be involved?** 

- Customer product owner and deployment architect 
- IBM Sales and Sales Engineers, Customer Success Managers 
- IBM Services  
  - [Build **watsonx**.ai ](https://ibm.seismic.com/Link/Content/DCJmjQ72TQGVGGCGWpRPpV74MFQG)
  - [Build **watsonx**.governance ](https://ibm.seismic.com/Link/Content/DCFmc2WfqmmTqGMJhTRjhVccJGQ3)
  - [Expertise Connect ](https://ibm.seismic.com/Link/Content/DC28j7HmTC7VbG2JXW6WQJb9h4m3)

**What information is needed about the existing CPD deployment?**   

- Owned VPC’s 
- Deployed VPC’s 
- Products and services used  
- Products and services FROM and TO sizing 
- Growth considerations for both CPD and new watsonx environments 

**How do I validate deployment configurations?** 

- Validate As-Is and To-Be CPD and watsonx.ai and .governance deployment configurations with licensing consumption detail and configurator on Seismic 
- Tech resources can help - Use *cpd-cli manage get-cr-status to get full view of current CPD environments* 

**What is the migration process?** 

**Confirm who executes migration** 

- Mandatory Plan TEL services leads   
- Recommended Migration TEL services leads 
- Customer staff  

**Confirm migration timeline**   

- Confirm services and customer agree to the migration timeline, with special focus on any ending dates synching migration and licensing 

**Confirm setup, import/export and testing strategy and planned completion dates**  

- Determine how will customer test and validate both updated As is environment and new To be environment 
- Does the planned project and completion fit with the commercial details? 

**Price offering** 

- Price Trade-up or Add-on parts with obtained required approvals if necessary 
- Price Mandatory and Recommended service parts  

**Positioning of watsonx and Cloud Pak for Data Software** 

**Are watsonx and Cloud Pak for Data both AI and data platforms?**  

1. watsonx is IBM’s AI and data platform (watsonx.ai, watsonx.governance, watsonx.data) designed for AI development, AI governance, and data lakehouse use cases 
1. While both watsonx and Cloud Pak for Data offerings include some of the same traditional AI tooling (non LLM), such as Watson Studio and OpenScale: 
- Cloud Pak for Data is the core of IBM’s Data Fabric, and is key to our customers finding, delivering, and using high quality, integrated, and trusted data sets in a variety of use cases. 
- The watsonx AI and data platform spans several core use cases, including generative AI/LLM foundation models and complete AI Governance across traditional and generative AI (e.g., AI builder tooling, AI governance, data lakehouse). 
3. You do not need to choose between watsonx and Cloud Pak for Data. They are often used together. For example, watsonx.data is often paired with IBM Knowledge Catalog (from Cloud Pak for Data) to add data enrichment and policy enforcement to data stored in open file formats and open table formats, including Parquet and Iceberg. 

**What are Data Services?** 

Data Services are a collection of offerings from IBM that enable clients to store, define, organize, manage, and deliver trusted data to train and tune AI models. 

**Do I need to choose between watsonx or Cloud Pak for Data? Can the offerings be used together?** 

It depends on the use case(s): 

Cloud Pak for Data is designed to address Data Fabric use cases 

watsonx is IBM’s AI and data platform (watsonx.ai, watsonx.governance, watsonx.data) designed for AI development, AI governance, and data lakehouse use cases.  

While clients may choose watsonx or Cloud Pak for Data depending on their use case(s), clients can also use watsonx and Cloud Pak for Data together. For instance, you can pair watsonx.ai and IBM Knowledge Catalog in Cloud Pak for Data to make it easier for data scientists to find trusted data to use in their AI model training. Cloud Pak for Data and watsonx can be deployed together on the same OpenShift cluster. 

**Where can I find a list of services included in Cloud Pak for Data and watsonx?** 

1. Services list for Cloud Pak for Data:[ https://www.ibm.com/docs/en/cloud- paks/cp-data/4.8.x?topic=integrations-services ](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.8.x?topic=integrations-services)
1. License and entitlements docs for watsonx.data: [https://www.ibm.com/docs/en/watsonxdata/1.0.x?topic=planning-licenses- entitlements ](https://www.ibm.com/docs/en/watsonxdata/1.0.x?topic=planning-licenses-entitlements)
3. watsonx.ai includes the traditional data science services in Cloud Pak for Data (e.g., Watson Studio, Watson Machine Learning, Watson Machine Learning Accelerator, Analytics Engine for Apache Spark, SPSS Modeler, etc.) plus new Generative AI tooling capabilities (e.g., Prompt Engineering).  

**What are common use cases for cross-selling Cloud Pak for Data and watsonx?** 

Cloud Pak for Data and Manta have natural cross-sell points with all three watsonx components. Additionally, watsonx.data has native integrations with DataStage and with Optim Archive Viewer, so these are good options for cross-sell opportunities. 

- Generative AI, as well as classic data science and machine learning, requires high quality inputs to train models. Without trusted data, you cannot produce trusted AI. 
- AI Governance focuses on measuring and managing the quality of AI models and their decisions, including foundation models. There is significant value in doing this purely at the model layer through techniques like drift/bias detection. However, a true end-to-end solution requires tracing the lineage of data sets used to build and train the model, all the way from source systems through integration and cleansing. This latter capability is part of the Data Fabric. 
- Lakehouses are naturally built to house a wide spectrum of data and operate at very large scale. These are the key ingredients of a flexible, modern data platform. They are also the key ingredients of sprawling, unusable data estates that lack governance and trust. Data governance technologies from the Data Fabric are therefore critical to the success of real-world Lakehouse implementations. Data Integration technologies are key to unlocking the value of the raw data assets ingested by the Lakehouse. 

**How should I position the data science capabilities in Cloud Pak for Data versus watsonx.ai and/or watsonx.governance?** 

watsonx should be positioned for all data science and AI opportunities. While there are data science capabilities in Cloud Pak for Data Enterprise Edition (commonly referred to as “base”), our generative AI development and AI governance capabilities will **NOT** be included in Cloud Pak for Data. Existing Cloud Pak for Data customers will not lose their data science capabilities, however, we anticipate that most customers will want to extend into Generative AI capabilities over the coming months and quarters. 

**How are IBM Knowledge Catalog and watsonx.governance positioned?** 

IBM Knowledge Catalog (formerly known as Watson Knowledge Catalog) is a data catalog service for data governance use cases (e.g., data discovery, data quality, data policies, self-service data catalog, etc.). Watsonx.governance is for AI governance use cases (e.g., AI model lifecycle, AI explainability, etc.). The two can be used separately, or combined to extend the visibility of AI Governance all the way back to the lineage of the data sets used to train/tune models. 

**How are Watson Query and watsonx.data positioned?** 

Watson Query is positioned to support data fabric through the logical data warehouse use case. It handles federation of traditional data warehouses well with pushdown optimizations. Watson.data is a data lakehouse that is designed to handle big data use cases with some federation capabilities. It pushes data consolidation as it excels in querying and processing large amounts of data, as well as building integrations that enable fit-for-purpose engines to access the same copy of data. 

Watson Query is based on the Db2 engine. The watsonx.data SQL engine is based on Presto today, and has an extensible architecture that will support additional engines in the future. 

Watson Query (rebranding of Data Virtualization) is only available through the Cloud Pak for Data Enterprise Edition license. watsonx.data is only available through the watsonx.data license. 

**Can Cartridges be positioned alongside watsonx?** 

Yes. Cartridges can be positioned along watsonx and/or Cloud Pak for Data.  **Is Cloud Pak for Data going to be phased out?** 

As the prior answers indicate, Cloud Pak for Data and Data Fabric remain key to IBM’s overall vision for Generative AI as well as traditional enterprise data use cases. They are not being phased out. 

**Common Packaging And Pricing Questions** 

**If a client has entitlements for Cloud Pak for Data, how can they migrate to the watsonx platform?** 

1. Cloud Pak for Data (Enterprise Edition, Standard Edition, or Transition Edition) can be upsold to watsonx.ai and/or watsonx.governance Model Management. OpenPages VPCs can be upsold to watsonx.governance Risk & Compliance Foundation. For the OpenPages Application portfolio, upsell options exist specifically for OpenPages, Model Risk Governance, Operational Risk Management, and Regulatory Compliance Management. 
1. Upsell motions come in three flavours: 
   1. Perpetual S&S to Perpetual S&S: standard trade-up parts (to be listed in the Mod Engine) 
   1. Perpetual S&S to Subscription: standard SL Upgrade parts (to be listed in the Mod Engine) 
   1. Subscription to Subscription: this was not previously possible, but a new Subscription License Add-on offering allows owners of a Cloud Pak for Data Subscription License to add watsonx capabilities on top for the remainder of their term.  
1. Some upsell options are marked as “Transition Editions”. These are exclusive to trade-up/upgrade/add-on sales and can not be sold net new. They differ from the regular watsonx editions in that the user retains the entitlement they owned before the trade-up. This enables watsonx upsells to provide an indefinitely long migration window off of the prior technologies, similar to the Modernization parts that were used to trade customers from standalone to Cloud Pak. 

**Common Product Technical Questions** 

**Can Watsonx.ai be transitioned or installed under new Licensing  without a new installation?** 

This is not recommended.**  Also , see note from Wx.ai Installation Doc below  

- If still desire to explore further then:  
  - Requires watsonx Brand Approval  
  - Software stack must be confirmed on supported releases  

**Can watsonx.gov be transitioned or installed under new licensing without a new installation**  

This is not recommended 

**Where can I find the latest version of the watsonx product roadmap?** 

watsonx product roadmap Seismic[ link.](https://ibm.seismic.com/Link/Content/DCMmpHHmJchDq8qW3dM9TX8qjW9d)  

**Can Cloud Pak for Data data fabric use cases be integrated with watsonx?** 

1. Data Fabric and watsonx.data are linked through two primary integrations. The first which was released in September 2023 allows for the application of Data Fabric Governance and Protection to data in watsonx.data. Essentially, Cloud Pak for Data users can connect to the tables in watsonx.data and then catalog them in IBM Knowledge Catalog. Once the data has been cataloged and profiled, users can then enforce Knowledge Catalog data protection rules within watsonx.data's Presto engine. This allows for IBM Knowledge Catalog to be a central catalog and access control center which then manages and protects data as it is accessed and consumed in watsonx.data. 
2. Alongside that primary integration, there will also be a new LLM based semantic automation layer released later in 2024 which will be used by IBM Knowledge Catalog and Watsonx.data to semantically enrich data across the systems--finding meaning, relationships, and descriptions in data — and then provide a LLM-based chatbot for conversational data search. This semantic automation layer will automate large portions of the data governance process and will greatly increase the time to value for data consumers by helping them to rapidly find the right data. 

**How are infrastructure footprint costs impacted when deploying various combinations of watsonx, Cloud Pak for Data, and Cartridges?** 

1. Infrastructure costs are driven by hardware, network, and storage along with FTE operational costs. In a typical deployment the monthly FTE operational costs are higher than the total monthly hardware, network, and storage costs. 
1. Combinations of watsonx, Cloud Pak for Data, and Cartridges typically do not materially increase FTE operational costs, however, some clients may choose to leverage OpenShift tenancy model (i.e., projects/namespaces) to simplify management operations: 
- Update products independently and maintain different levels of maturity. This is important to our clients because they typically upgrade software versions for AI deployments more frequently than they upgrade software for data governance workloads. 
- Improve security posture by deploying in separate tenants. 
- Simplify license management and internal chargebacks. 
- Align with standard OpenShift deployment best practices (e.g., deploying Cloud Paks in separate projects). 
3. The primary driver of incremental infrastructure costs for watsonx.ai deployments is the requirement for GPUs to run Generative AI workloads. 

**Can watsonx and Cloud Pak for Data be deployed in the same namespace?** 

1. watsonx and Cloud Pak for Data are designed to be deployed in separate namespaces. For example, guidance on installing watsonx.ai is available here: [https://www.ibm.com/docs/en/cloud-paks/cp-data/4.8.x?topic=watsonxai- installing ](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.8.x?topic=watsonxai-installing)
2. While watsonx and Cloud Pak for Data are built on a common framework, they are separate products with different workload profiles (e.g., GenAI on GPUs, lakehouse storage, etc.). Reasons why clients may desire to deploy watsonx and Cloud Pak for Data as separate tenants (i.e., within separate projects/namespaces) include: 
- Updating products independently and maintaining different levels of maturity. This is important to our clients because they typically upgrade software versions for AI deployments more frequently than they upgrade software for data governance workloads. 
- Improving security posture by deploying in separate tenants. 
- Simplifying license management and internal chargebacks. 
- Aligning with standard OpenShift deployment best practices (e.g., deploying Cloud Paks in separate projects). 

**Is there a cohesive detailed technical architecture that covers Cloud Pak for Data, Data Fabric, and watsonx?** 

1. Please see the Cloud Pak for Data Architecture docs pages: [https://www.ibm.com/docs/en/cloud-paks/cp-data/4.8.x?topic=planning- architecture ](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.8.x?topic=planning-architecture)
1. The watsonx deployment architecture docs are here: [https://www.ibm.com/docs/en/cloud-paks/cp-data/4.8.x?topic=watsonxai- installing ](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.8.x?topic=watsonxai-installing)

**What is the interoperability between IBM Knowledge Catalog and watsonx.data?** 

A connection asset (watsonx.data[ connection)](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.7.x?topic=catalogs-watsonxdata-connection) can be created from IBM Knowledge Catalog to govern watsonx.data data sources. 

**Can LLMs be run on both Cloud Pak for Data and watsonx?** 

Technically, LLMs can be developed on both Cloud Pak for Data and watsonx if the user develops the LLMs through native IDEs (e.g., Jupyter notebooks). However, very few clients would choose to take this approach given how difficult it would be to manage the lifecycle of the LLM without having watsonx.ai and watsonx.governance. **We recommend all LLM development to happen on the watsonx platform**. IBM will not support LLMs via legacy Cloud Pak for Data capabilities (or e.g. Watson Studio).  

**Is there an integration available between Data Fabric offerings and Snowflake (data movement, data quality, etc.)?** 

There is a connector so you can do ETL/ELT (DataStage) with Snowflake, DQ rules with IBM Knowledge Catalog, metadata import, etc. 

**Is there any planned development in watsonx.data SQL pushdown and improving data gravity affinity?** 

The Product team is currently investigating options for bringing SQL pushdown to watsonx.data. 

**Are there any planned developments in applying AI to data quality?** 

Yes. As part of the further adoption of Generative AI in Cloud Pak for Data and watsonx, IBM Knowledge Catalog Data Quality will be enhanced through two new major AI integrations coming in 2024. In the 1H release we will providing Data Quality Rule auto-generation, this will use AI to auto-suggest straightforward DQ Rules based on the data.  

**Will the storage certification be the same between watsonx and Cloud Pak for Data?** 

Yes, both products are following the same storage certification process and validating against the same set of requirements. For more information, see the documentation on Storage Considerations:[ https://www.ibm.com/docs/en/cloud-paks/cp- data/4.8.x?topic=planning-storage-considerations ](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.8.x?topic=planning-storage-considerations)

**Is IBM Storage Scale Container Native supported by watsonx.ai?** 

Yes, it is supported by watsonx.ai, as it is across the platform: [https://www.ibm.com/docs/en/cloud-paks/cp-data/4.8.x?topic=planning-storage- considerations ](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.8.x?topic=planning-storage-considerations)
