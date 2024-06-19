![](Aspose.Words.6dfa5d92-4834-4519-bbea-aaffcee4f572.001.png) ![](Aspose.Words.6dfa5d92-4834-4519-bbea-aaffcee4f572.002.png)

Competitive Information         **Recent announcements summary – June 2023** 

**INDIVIDUAL ANNOUNCEMENTS AND PRELIMINARY ANALYSIS** ![](Aspose.Words.6dfa5d92-4834-4519-bbea-aaffcee4f572.003.png)

Databricks recently made several announcements at their Data + AI Summit (June 26-29, 2023), this document provides a summary of these new features and capabilities along with competitive analysis from an IBM watsonx.data perspective. The key news was in the areas of Delta Lake and Unity Catalog. Each announcement will contain a technical overview of the feature or capability, its status (including a tentative release data if available), and a competitive analysis compared to watsonx.data. 

Lakehouse federation capabilities in Unity Catalog 

The Unity Catalog within Databricks will be enhanced to allow federation with data sources outside of Databricks. MySQL, PostgreSQL, Amazon Redshift, Snowflake, Azure SQL Database, Azure Synapse, Google’s BigQuery, and more data sources can be managed within the Databricks Unity Catalog without moving or copying the data. 

The requirement for unified governance is to reduce data fragmentation across data sources. There are three primary results of data fragmentation; it is difficult to discover and access all data, slow execution due to data engineering bottlenecks as the data must be moved from the external source to the platform of choice, and weak compliance across siloed systems leading to duplication of effort which increases the risk of monitoring and protecting data from unauthorized access. 

![](Aspose.Words.6dfa5d92-4834-4519-bbea-aaffcee4f572.004.jpeg)

Lakehouse federation within Unity Catalog will provide data discovery and classification of all data in a single location, accelerate ad-hoc analysis and querying of your data with a single engine. This includes advanced query planning across data sources and caching ensures optimal query performance even when accessing and combining data from multiple platforms with a single query. There is a single permission model to set and apply access and safeguard all data sources. With the new capability, Unity Catalog can discover, govern, and query data across data platforms including MySQL, PostgreSQL, Amazon Redshift, Snowflake, Azure SQL Database, Azure Synapse Analytics, Google BigQuery, and more without having to move or copy data. 

- **Status** – Private preview (beta) for limited Databricks clients with public preview projected to begin in July 2023. General availability (production use) is projected to be Q4 2023 or Q1 2024. 

Competitive analysis 

The ability to govern data sources outside of Databricks is much needed enhancement to the existing Unity Catalog component of Databricks. Since this capability is in private preview, documentation and technical details are not yet available to allow a detailed analysis of the lakehouse federation capabilities within Databricks Unity Catalog. However, based on the data sources listed and the information provided in this Databricks[ blog,](https://www.databricks.com/blog/introducing-lakehouse-federation-capabilities-unity-catalog) this solution appears to be limited to a multi-cloud environment. This capability will be useful for clients that have all their data sources within public clouds supported by Databricks (Amazon Web Services (AWS), Microsoft Azure, and Google Cloud Platform (GCP)). However, for clients that have data lakehouses that have data sources on other clouds or utilize a hybrid cloud environment, the Unity Catalog Lakehouse Federation capability will not provide a single data catalog and data governance platform. For these clients, watsonx.data and IBM Watson Knowledge Catalog (WKC) will provide a single data source catalog and data governance solution. 

- **Competitive assessment for IBM watsonx.dat**a – Advantage for IBM with a data governance solution that supports hybrid cloud environments and delivers a single data governance solution for a data lakehouse environment. WKC has been in production for several years and is more mature than Databricks Unity Catalog with its new federation capability. 

Delta Lake 3.0 with new Universal Format and Liquid Clustering Universal Format (UniForm) 

Databricks has announced Delta Lake 3.0 as a release candidate (preview) in the open-source community (available for client download) and provides the initial implementation of the new Universal Format within Delta Lake. UniForm provides the ability for Apache Iceberg clients to read a Delta Lake table that has been configured for UniForm. Apache Iceberg clients can access the Delta table in read-only mode, with no data conversion needed. Databricks discusses the new Delta Lake 3.0 capabilities in this [blog.](https://www.databricks.com/blog/announcing-delta-lake-30-new-universal-format-and-liquid-clustering) Although the blog mentions that Delta Lake 3.0 UniForm will support both Apache Iceberg and Hudi reads on Delta Parquet files, the initial release is limited to Apache Iceberg support, which is detailed in this[ preview document.](https://github.com/delta-io/delta/releases/tag/v3.0.0rc1) Delta tables within Databricks must be created with the universal table format option to allow UniForm table access defined, this is not the default behavior for Delta tables. To change existing Delta tables to UniForm tables, both the UniForm option and table column-mapping must be enabled to use UniForm. More details about enabling Delta tables for UniForm access are found in the UniForm [documentation.](https://docs.delta.io/3.0.0rc1/delta-uniform.html) Once a Delta table is created or converted to a UniForm table, all writes to the Delta table must use Delta Lake 3.0. UniForm does not allow Databricks to read Apache Iceberg tables, it allows Delta tables to be read by Apache Iceberg clients. Future plans on whether Databricks would read native Apache Iceberg tables in the future were not mentioned in the blog.  

The mechanism that Databricks used to allow Delta tables to be read by Apache Iceberg clients is to add metadata to the file definition that can be understood by Apache Iceberg. Based on performance testing that Databricks has done with Delta Lake 3.0 UniForm tables, the overhead of maintaining this additional metadata during table writes is negligible.  

![](Aspose.Words.6dfa5d92-4834-4519-bbea-aaffcee4f572.005.jpeg)

In addition, a Delta table enabled for Apache Iceberg reads has better read performance than a native Iceberg table due to an improved internal layout of data within the Delta table (compared to a native Apache Iceberg table) written by Delta UniForm. 

- **Status** – Currently in preview (July 2023) with no projected release date or information on when Hudi support will be added to Delta Lake 3.0 UniForm 

Liquid Clustering 

As part of the Delta Lake 3.0 announcement, Databricks discussed the concept of Liquid Clustering. Liquid Clustering simplifies getting the best query performance with cost-efficient clustering as the data grows with the lakehouse. Although Liquid Clustering is mentioned as a key capability in the announcement blog, the capability is NOT in preview at the present time (July 2023) and listed as “coming soon”. Here are additional details about Liquid Clustering that was provided by Databricks: 

“*Liquid Clustering is a smart data management technique for Delta tables. It is flexible and automatically adjusts the data layout based on clustering keys. Liquid Clustering dynamically clusters data based on data patterns, which helps to avoid the over- or under-partitioning problems that can occur with Hive partitioning.* 

- *Liquid is simple: You set Liquid clustering keys on the columns that are most often queried - no more worrying about traditional considerations like column cardinality, partition ordering, or creating artificial columns that act as perfect partitioning keys.* 
- *Liquid is efficient: It incrementally clusters new data, so you don't need to trade-off between improving performance with reducing cost/write amplification.* 
- *Liquid is flexible: You can quickly change which columns are clustered by Liquid without rewriting existing data.”* 

Above information (in *italics*) was provided by Databricks in this[ blog ](https://www.databricks.com/blog/announcing-delta-lake-30-new-universal-format-and-liquid-clustering)post. 

Here are some performance charts (preliminary) highlighting the advantages of Liquid Clustering in a Delta environment. 

![](Aspose.Words.6dfa5d92-4834-4519-bbea-aaffcee4f572.006.jpeg)

- **Status** – Currently announced with only a “coming soon” status in the Delta Lake 3.0 preview documentation. 

Delta Kernel 

Although not mentioned by name in the announcement blog title, the blog contents mention another Delta Lake 3.0 new capability, Delta Kernel. Delta Kernel will simplify the building of Delta connectors by providing simple, narrow programmatic Application Programming Interfaces (APIs) that hide the complex details of the Delta protocol specification. The purpose of Delta Kernel is to make it easier for integrators to work with Delta Lake, when changes are made to Delta Lake, simply update the Delta Kernel and all new capabilities are inherited by the connectors. There are no coding changes required, and combined with Delta Lake UniForm that updates the table metadata for Apache Iceberg and Hudi readers means that once an engine integrator updates for Delta, they are automatically updated for the other open table formats. 

- **Status** – Currently in preview (July 2023) with no projected release date. 

Competitive analysis 

Delta Lake 3.0 and its new capabilities will assist Databricks in satisfying client requirements to utilize multiple open table formats. The ability to read Delta Parquet files from Apache Iceberg and Hudi clients without having to perform any conversion effort and still being able to read and write to the underlying Delta table may be an important capability for some clients. There are  restrictions and limitations currently with the UniForm capability that may render it unusable for some clients. UniForm allows only read access from non-Delta Lake clients, so it is good for Databricks clients that want to share data with suppliers or partners that utilize Apache Iceberg or Hudi as their open table format. UniForm does NOT allow Databricks clients to easily read data from their partners or suppliers that utilize other open table formats, so the long-term benefit to clients currently using (or considering) Databricks remains to be seen. 

Like the Delta Lake 3.0 UniForm, the advantage of Delta Kernel is the long-term is yet to be determined. Although updating Delta Kernel instead of updating connector code when a new version is released is beneficial, the benefit is limited to Databricks clients. The long-term benefit depends on how many Delta connectors clients are building today as to whether this will save significant time and cost when new releases of Delta Lake are available. 

The Liquid Clustering capability can be significant if table partitioning selection and overall query performance for Databricks improves significantly. With the capability not yet in preview and only preliminary data points available it is difficult to predict the overall impact of Liquid Clustering in increasing Databricks market share and adoption rate. 

- **Competitive assessment for IBM watsonx.data** – IBM watsonx.data has the benefit of being more open than Databricks and with Apache Iceberg being favored by a larger number of lakehouse vendors than Delta Lake, it remains to be seen if Delta Lake 3.0 will increase adoption of Delta Lake outside of Databricks and Microsoft Azure. Providing the ability to at least read Delta Parquet files with watsonx.data would provide a comparable capability and should be included on the watsonx.data roadmap for the future.   

**SUMMARY ![](Aspose.Words.6dfa5d92-4834-4519-bbea-aaffcee4f572.007.png)**

The announcements that Databricks made during the Data + AI Summit in late June 2023 around their Unity Catalog and Delta Lake 3.0 capabilities highlight that Databricks is a formidable competitor in the data lakehouse market.  

Compared to IBM Watson Knowledge Catalog, Databrick Unity Catalog does not offer a hybrid cloud governance capability and is only catching up around multi-cloud data governance. Overall, IBM has a leading data governance solution with Watson Knowledge Catalog and tighter integration with watsonx.data will ensure that IBM has the edge in this technology. 

The Delta Lake 3.0 UniForm that adds metadata for Apache Iceberg and Hudi to Delta tables to allow seamless reads against Delta tables by Apache Iceberg and Hudi clients was a needed capability for Databricks but does not provide a competitive differentiator to choose Delta Lake over Apache Iceberg as an open table format. Delta Lake is still primarily controlled by Databricks and the ability to read Delta tables from Apache Iceberg and Hudi clients does not make the open table format less closed. 

The Liquid Clustering capability (if it works as advertised) could improve Databricks competitive position from a query performance and cost optimization perspective, but further analysis and understanding of the technology (once it is available and documented) is required to complete a competitive assessment. 
© 2023 IBM Corporation  For comments and questions, please contact Danny Arnold (darnold@us.ibm.com)
