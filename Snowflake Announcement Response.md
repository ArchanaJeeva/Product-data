![](Aspose.Words.e3429f99-12d3-4b15-977b-a4e92dcae3b5.001.png) ![](Aspose.Words.e3429f99-12d3-4b15-977b-a4e92dcae3b5.002.png)

Competitive Information         **Recent announcements summary – June 2023** 

**INDIVIDUAL ANNOUNCEMENTS AND PRELIMINARY ANALYSIS** ![](Aspose.Words.e3429f99-12d3-4b15-977b-a4e92dcae3b5.003.png)

During their recently concluded Snowflake Summit (end of June 2023), Snowflake made a number of announcements that provided insights into their direction and priorities for the near term. There were several announcements made by Snowflake, here are the more impactful announcements from an IBM viewpoint: 

- Managed Iceberg Tables  
- Dynamic Tables 
- Snowpipe Streaming API 
- AI-related announcements 
- Nvidia partnership 
- Snowflake Copilot 
- Document AI (based on Applica acquisition) 

Each of these announcements will be covered in more detail in this competitive document. 

Although not directly related to improving Snowflake functionality or capabilities, Snowflake announced Budgets to improve cost optimization and better control a client’s Snowflake spend. This is an area worth discussing with potential clients in a competitive sales situation, as IBM has been discussing how costs can exponentially increase for Snowflake clients as their data warehouse environments grow and they must contend with peak workload periods using Snowflake scale up and scale out technology.  

Managed Iceberg Tables  

Prior to 2022, Snowflake only supported Apache Iceberg tables as read-only external tables, which do not perform as well as standard Snowflake tables. At Snowflake Summit 2022 (a year ago), Snowflake announced support for Apache Iceberg that allowed Snowflake to access Iceberg tables as another Snowflake table while clients benefited from using the Snowflake high- performance query engine for compute. Since Iceberg tables were now treated as Snowflake native tables, all table activity (insert, update, delete, and select) was allowed. However, these tables were not managed by Snowflake and required the Iceberg metadata to be kept updated using a separate catalog (versus the native Snowflake catalog). With the recent Snowflake Summit 2023 announcement, Snowflake now offers managed Iceberg tables, a “managed” Iceberg table includes Snowflake updating the Iceberg catalog as required, providing a complete Iceberg table solution (no need for separate Iceberg catalog maintenance). 

Here is a diagram that illustrates managed Iceberg tables within Snowflake. 

![](Aspose.Words.e3429f99-12d3-4b15-977b-a4e92dcae3b5.004.jpeg)

- **Status** – Private preview (no date specified for public preview period). 

Competitive analysis 

Managed Iceberg tables are a benefit to clients if Snowflake is their primary access method for data contained in Iceberg tables. For clients that use other query engines against Iceberg tables along with Snowflake, clients will now be forced to access Iceberg tables through Snowflake (as the Iceberg catalog is being managed by Snowflake), which will increase a client’s compute charges for data access. Using Snowflake managed Iceberg tables does not allow clients to utilize other query engines with their Iceberg tables (unless that other query engine can work within the Snowflake environment), preventing them from cost optimizing the compute component of their data lakehouse.  

Although documentation is not available due to this feature being in private preview, the diagram appears to indicate that you are altering the Iceberg table to now be included in the Snowflake catalog. This makes it appear that managed Iceberg tables is a migration process versus a coexistence environment. The diagram has “CONVERSION” in its title, making it seem to be a one- way process moving away from the native Iceberg catalog. This feature will need to be examined closer upon release to public preview, as a Snowflake managed Iceberg table may not be able to be accessed by watsonx.data (unless Snowflake opens access to the Snowflake catalog to other entities like watsonx.data). 

IBM watsonx.data can utilize either Db2 or Netezza Performance Server (NPS) data warehouse query engines in addition to Ahana Presto and Apache Spark query engines for a complete data lakehouse environment that does provide cost optimization of the compute component of the lakehouse. 

Dynamic Tables 

One of the biggest transformation cost drivers for current Snowflake clients is the fact that tables need to be rebuilt every time a data pipeline is run. This is because it is quicker and easier to rebuild a data pipeline versus incrementally updating a table. If data pipelines are run on a simple schedule without considering other factors, a data pipeline might be executed just prior to a large data update occurring which means that the data pipeline will have to be executed again to account for the last minute data update. Clients could use materialized views (MVs) within Snowflake to address some of the issues around data pipelines and allow tables to be updated only when new data arrives. However, there were restrictions around MVs such as the SQL view definition could not include common operations such as joins, unions, aggregations, group bys, or window functions. With Dynamic Tables, Snowflake allows SQL view definitions without the restrictions of MVs to make easier for clients to build and maintain data pipelines.  

The chart below highlights the advantages of Dynamic Tables within Snowflake. 

![](Aspose.Words.e3429f99-12d3-4b15-977b-a4e92dcae3b5.005.jpeg)

- **Status** – Public preview with no date provided for general release. 

Competitive Analysis 

This feature will reduce the manual effort of existing Snowflake clients in maintaining data pipelines but does not provide any capabilities that are not available within the IBM ecosystem for a data lakehouse. In addition to watsonx.data capabilities, IBM offers other products and services to assist clients in managing and creating data pipelines that are not restricted to only a single data warehouse environment. It is important to remember that Snowflake has a single data warehouse query engine and a proprietary environment that limits a client to the Snowflake ecosystem and only public cloud deployment options. IBM provides a broader hybrid cloud solution and an open ecosystem with the watsonx platform and delivers compute cost optimization along with storage cost savings for data lakehouse environments with watsonx.data. 

Snowpipe Streaming API 

Snowflake announced their new Snowpipe Streaming Application Programming Interface (API) that allows clients to load data directly into Snowflake from Apache Kafka or a custom Java application. Snowpipe Streaming is the most cost effective way to load data once you have the necessary infrastructure in place. Alternative data loading strategies like Snowpipe or manual COPY INTO statements running on a self-managed database (or other data source) both involve loading a file into Snowflake. By avoiding the expensive read step and file management overhead, Snowpipe Streaming becomes a more cost-effective option. 

This diagram highlights the Snowpipe Streaming capability. 

![](Aspose.Words.e3429f99-12d3-4b15-977b-a4e92dcae3b5.006.jpeg)

- **Status** – Public preview with no announced release date. 

Competitive Analysis 

This is not a new capability from a competitive standpoint, it is another capability that Snowflake has added to try and reduce costs for clients. From an IBM perspective, data warehouse offerings like Netezza Performance Server (NPS) has provided the ability to use Apache Kafka for over a year, while Snowflake is positioning this as a new capability that is only available currently in public preview for Snowflake. 

AI-related announcements 

This portion of the document will cover these AI-related announcements; Nvidia partnership, Snowflake Copilot, and Document AI. 

Nvidia partnership 

Snowflake will partner with Nvidia to integrate Nvidia’s Large Language Model (LLM) framework NeMo into Snowflake. This will assist clients that want to build large language models directly into Snowflake, using data that is already stored in Snowflake. 

- **Status** – Partnership finalized and announced in June 2023. 

Snowflake Copilot 

Snowflake Copilot is a “comment to SQL” feature that will allow a client to enter a comment like “—show me the count of active users over the last 30 days”. Snowflake will then automatically generate the query using its knowledge of a client’s data and the exact Snowflake SQL dialect. Snowflake has a large data set of queries that will enable them to train Copilot feature.  

- **Status** – Announced and provided a small demonstration, but there is no Private preview or Public preview timeframe provided by Snowflake. 

Document AI 

Snowflake announced a new product, Document AI that is derived from their April 2022 acquisition of Applica which specialized in processing unstructured data. Document AI is Snowflake’s first party LLM and lets clients ask questions about documents that are stored in Snowflake. Document AI will retrieve information from documents and then ask clients to provide feedback on the information retrieved to further refine the model. 

- **Status** – Private preview (no date specified for public preview period). 

Competitive analysis 

Here is a competitive analysis of each of the AI-related announcements from Snowflake.  

- **Nvidia partnership** – This partnership will provide a LLM framework to Snowflake but restricts clients from using any LLMs for any data that is external to Snowflake. Snowflake is continuing their strategy of trying to expand a client’s usage of Snowflake virtual warehouse as the sole query engine and lock-in clients to a Snowflake-centric ecosystem. IBM watsonx.ai provides a more open AI solution for clients and is integrated into the overall watsonx platform that includes data sources and data governance for a more robust solution than the data warehouse centric Snowflake solution. 
- **Snowflake Copilot** – The “comment to SQL” feature seems like a basic, restrictive version of IBM semantic automation that is available in watsonx.data. But Snowflake Copilot follows the Snowflake strategy of ensuring all data is contained in Snowflake versus the ability to access and provide augmented information about all data sources that is possible with IBM watsonx.data semantic automation. IBM watsonx.data has the advantage over Snowflake for this capability. 
- **Document AI** – This product will provide additional functionality to Snowflake clients if the documents that a client wants to ask questions about exists in Snowflake. The continual Snowflake strategy of forcing clients to place all data in Snowflake to use new tools and capabilities is not in the best interests of clients and a lock-in platform severely limits a client’s ability to adapt their data platform solution as future business requirements warrant. IBM watsonx.data and IBM watsonx.ai provide a more open and adaptable solution around AI and data than what Snowflake is offering clients. 

Other announcements – Budgets 

One of the challenges for Snowflake clients that has been discussed from a competitive perspective by IBM when encountering Snowflake in competitive sales situations is the double cost impact of Snowflake scale up and Snowflake scale out. Snowflake scale up always provides 2x the compute resources of the previous T-shirt size virtual warehouse when additional compute is required for increased query complexity and/or increased data volume. Snowflake scale out provides compute resources for query concurrency and prevents queries from queuing within Snowflake (which adversely impacts overall query performance by increasing the elapsed time of each query that is queued) by provisioning additional virtual warehouse clusters from 1 cluster up to a total of 9 clusters (for a total of 10 virtual warehouse clusters), where each scale out virtual warehouse cluster increases a client’s cost by 100% (for example, a total of 4 virtual warehouse clusters increases the Snowflake client subscription cost by 400% or 4x that of the original virtual warehouse cluster). Snowflake has tried this cost optimization issue by providing resource monitors which allow a client to control how many total Snowflake credits (1 credit = 1 server per hour) are consumed by a virtual warehouse cluster or group of virtual warehouse clusters (a Snowflake scale out environment) within a month. At Snowflake 

Summit 2023, Snowflake announced a new tool to allow clients to budget their Snowflake spend, Budgets. Budgets extend the cost optimization capabilities by allowing clients to control the compute resources used by allowing them to group Snowflake resources into categories or groups such as virtual warehouses, tables, Snowpipes, materialized views, and other resources. A 

client can then specify the maximum resources for each usage category to provide more granular control over their Snowflake spend than was possible with resource monitors alone. Both resource monitors and Budgets allow clients to either be alerted about budget overages or suspend processing to prevent going over budget. 

- **Status** – Public preview with no date provided for general release. 

Competitive analysis 

If Snowflake did not have these cost issues, why is Budgets yet another tool provided by Snowflake to control costs and client spend (not to mention tools provided by other vendors to assist clients in controlling Snowflake costs and keep in budget)? Combine the difficulty in controlling costs within Snowflake with the reality that Snowflake is limited to a single high-cost, high- performance query engine versus the multiple query engine capabilities of IBM watsonx.data that allow a client to choose a high- performance query engine for applications and queries that require it while allowing a lower cost compute query engine to be used for workloads that do not require maximum performance within the data lakehouse. Snowflake is a closed, high-cost environment that provides little flexibility for clients as their data processing requirements change over time versus the open IBM watsonx environment that provides hybrid cloud deployment options and client choice to optimize compute and storage cost depending on individual workload requirements. 

**SUMMARY ![](Aspose.Words.e3429f99-12d3-4b15-977b-a4e92dcae3b5.007.png)**

The announcements that Snowflake made during the Snowflake Summit 2023 in late June 2023 highlight that Snowflake is continually working to improve their product and address client concerns and overcome shortcomings within Snowflake. 

Snowflake’s managed Iceberg tables capability is in private preview and no public documentation or detailed explanation of the feature is available. Based on the limited information available and the diagram shown earlier in this paper, it appears that managed Iceberg tables converts an Iceberg table to internal Snowflake management and is therefore restrictive to clients that want to use other query engines other than Snowflake against Iceberg tables. This feature will require additional analysis after public preview is available to ensure external query engines (like watsonx.data Ahana Presto) will be have access to Snowflake catalog when a client uses Snowflake managed Iceberg tables or whether Snowflake catalog access is limited to Snowflake only. 

Snowflake Dynamic Tables are just an extension to their materialized views and do not provide any capabilities that provide a competitive advantage. This Snowflake capability is targeted to maintaining all client data within the Snowflake environment and allows no ability to access data outside of Snowflake tables providing another lock-in point for Snowflake. 

Snowpipe Streaming API is another “me too” capability that provides a catch-up capability for Snowflake that already exists in data warehouse platforms like IBM Netezza Performance Server (NPS). This capability does help Snowflake clients as it is a more cost-effective solution for loading data than using a staging file or table. 

Snowflake’s AI-related announcement highlight that Snowflake has no capabilities that other vendors do not provide and IBM watsonx provides a more open and complete data lakehouse and AI environment than Snowflake. 

Finally, the addition of Snowflake Budgets should focus a client’s attention on the fact that existing Snowflake customers do have a cost issue with Snowflake. If Snowflake had no cost issues, why do they have two tools (resource monitors and Budgets) to assist clients in controlling costs along with Snowflake budget and cost optimization tools from third-party sources. 
© 2023 IBM Corporation  For comments and questions, please contact Danny Arnold (darnold@us.ibm.com)
