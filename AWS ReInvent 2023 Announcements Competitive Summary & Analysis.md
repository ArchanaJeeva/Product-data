![](Aspose.Words.d0641802-ffd0-48e5-85aa-e6037c291563.001.png) ![](Aspose.Words.d0641802-ffd0-48e5-85aa-e6037c291563.002.png)

Competitive Information **Amazon Web Services (AWS) – Nov. 2023**

**INDIVIDUAL ANNOUNCEMENTS AND PRELIMINARY ANALYSIS** ![](Aspose.Words.d0641802-ffd0-48e5-85aa-e6037c291563.003.png)

Amazon Web Services (AWS) made a number of announcements in the areas of data warehouse and data lakehouse. Here is a summary of the announcements for these areas within AWS with a quick link provided for faster access to the details of each announcement. 

**Amazon Redshift**

*Amazon Aurora PostgreSQL and Amazon RDS MySQL zero-ETL integration with Amazon Redshift Multidimensional Data Layouts to optimize query performance*

*General Availability for Apache Iceberg Table Support*

*Amazon Q generative SQL in Amazon Redshift Query Editor*

*Metadata security to simplify multi-tenant applications*

*Multi-data warehouse writes through Data Sharing*

*Amazon Redshift Serverless AI-driven autoscaling and optimization*

*Incremental Refresh for Materialized Views on data lake tables*

*New Fine Grained Access Control (FGAC) to nested objects*

*Competitive analysis*

**Data Lakehouse**

*Amazon Athena support for Amazon S3 Express One Zone storage*

*AWS Glue Data Catalog supports generating column-level statistics*

*AWS Glue Data Catalog supports multi-engine views with AWS Analytics Engines Competitive analysis*

**Amazon Redshift** 

Amazon Aurora PostgreSQL and Amazon RDS MySQL zero-ETL integration with Amazon Redshift 

Integration between Aurora PostgreSQL and Amazon Redshift or Amazon RDS MySQL and Amazon Redshift allows clients to use transactional data for analysis in Amazon Redshift without having to build a data pipeline or a complex Extract, Transform, and Load (ETL) process. 

![](Aspose.Words.d0641802-ffd0-48e5-85aa-e6037c291563.004.jpeg)

*Figure 1 - Diagram illustrating zero-ETL integration between Amazon Aurora PostgreSQL and Amazon Redshift.* 

![](Aspose.Words.d0641802-ffd0-48e5-85aa-e6037c291563.005.jpeg)

*Figure 2 - Diagram illustrating zero-ETL integration between Amazon RDS for MySQL and Amazon Redshift.*

Important things to know

- This capability sets up replication automatically between the source Aurora PostgreSQL database or Amazon RDS MySQL database and the target Amazon Redshift data warehouse.
- There is no specific additional charge for using zero-ETL integration with Amazon Redshift, but the client may incur additional storage charges for maintaining the enhanced logging required for the replication process. If the source and target database are in different AWS availability zones, there will be data transfer charges as well.

NOTE: There is already zero-ETL integration between Amazon Aurora MySQL and Amazon Redshift and this capability is in production. 

Current status (GA, Public preview, or Private preview).

- Status – Public preview. 

Multidimensional Data Layouts to optimize query performance

Amazon Redshift does not provide indexes to improve performance like some other data warehouses. Although originating from the PostgreSQL code base, Redshift utilizes column-organized tables (versus the row-organized tables of open source PostgreSQL) and has sort keys to improve query performance. A sort key determines the order that the data rows are stored within a table, if a sort key is chosen correctly (based on the query workload), table data is accessed more efficiently (less I/O operations) and query performance is improved. Sometimes a table is not always accessed by the same column or columns, as there can be multiple queries that access a table, and the queries may utilize different columns within a table depending on the information the query requires. To address this situation, Amazon Redshift uses Multidimensional Data Layouts (MDDL). Instead of sorting table data within the table based on a sort key, MDDL sorts data based on the incoming query filters. This significantly accelerates the performance of table scans (as the data is sorted to accommodate the query column requirements). MDDL within an Amazon Redshift data warehouse works in conjunction with Automatic Table Optimization (ATO) capability within Amazon Redshift. To enable MDDL for a table, a client must set the SORTKEY attribute of the table to AUTO or enable ATO. Enabling ATO for the database will not guarantee the use of MDDL, ATO may choose to use a single sort key, or it may use MDDL, it depends on the workload. A client can query the SVV\_TABLE\_INFO system table and examine the SORTKEY1 column to verify if MDDL is being used for a table. 

![](Aspose.Words.d0641802-ffd0-48e5-85aa-e6037c291563.006.jpeg)

*Figure 3 - AWS provided performance information highlighting the benefits of MDDL usage.*

Important things to know

- Clients have to enable Automatic Table Optimization (ATO) for MDDL to be a data sorting option for a table, but whether MDDL is utilized depends on the workload and the sort key determination by ATO. A client cannot force MDDL to be used for a table, it is strictly workload dependent based on the ATO analysis of the workload.

Current status (GA, Public preview, or Private preview).

- Status – Public preview. 

General Availability for Apache Iceberg Table Support

Amazon Redshift provides full query support for Apache Iceberg tables. Clients can run transactionally consistent queries on Apache Iceberg tables providing full data lakehouse access from Amazon Redshift.

Important things to know

- Amazon Redshift can only read Apache Iceberg tables. For write transactions, clients must use the separately priced Amazon EMR, Amazon Athena, or AWS Glue services. 

Current status (GA, Public preview, or Private preview).

- Status – General availability (GA). 

Amazon Q generative SQL in Amazon Redshift Query Editor 

Amazon Q is part of the out of the box, web-based Amazon Redshift Query Editor to analyze query intent, query patterns, and schema metadata to identify common SQL patterns within Amazon Redshift to accelerate the query authoring process and reduce the time required to produce actionable data insights. People building queries can utilize natural language to ask questions and receive Structured Query Language (SQL) code recommendations.

Important things to know

- At the current time (December 2023), English is the only supported language for natural language interactions.
- Questions must reference data within the Amazon Redshift database, external schemas cannot be referenced.
- Due to the possibility of hallucinations with generative AI, it is recommended that any code suggested is well tested and validated prior to using the SQL in production.

Current status (GA, Public preview, or Private preview).

- Status – Public preview. 

Metadata security to simplify multi-tenant applications 

Metadata security is now supported to allow Amazon Redshift administrators to restrict the visibility on catalog metadata based on user roles and privileges. Amazon Redshift users will now see only databases, schemas, and tables/views for which they have been granted access. This enables clients to deploy multi-tenant applications on a provisioned Amazon Redshift cluster or an Amazon Redshift Serverless namespace.

Important things to know

- Can grant access to the database catalog without granting access to the underlying objects within the catalog.
- By default, the superuser role has access to the complete catalog for an Amazon Redshift database.

Current status (GA, Public preview, or Private preview).

- Status – General availability (GA). 

Multi-data warehouse writes through Data Sharing

This capability allows a client to write to an Amazon Redshift database from multiple Amazon Redshift data warehouses through the data sharing capability of Amazon Redshift. The data being written is visible to all data warehouses as soon as the transaction is committed. 

Important things to know

- This capability is only available on the two largest Amazon Redshift RA3 node sizes (ra3.4xl and ra3.16xl) and Amazon Redshift Serverless configurations.
- The least expensive and smallest Amazon Redshift RA3 node type, the ra3.xlplus, cannot use this new capability.

Current status (GA, Public preview, or Private preview).

- Status – Public preview. 

Amazon Redshift Serverless AI-driven autoscaling and optimization

Amazon Redshift Serverless now uses AI-driven autoscaling operations that will scale a data warehouse based on current workload characteristics such as data volume changes, concurrent queries, and query complexity. Amazon Redshift can adjust data warehouse scaling during the day based on workload patterns and changes.

Important things to know

- The AI-driven autoscaling operations are only applicable to Amazon Redshift Serverless, there is no ability to auto scale Amazon Redshift data warehouse fixed node size configurations. For example, clients that are using Amazon Redshift ra3.xlplus nodes cannot take advantage of this capability.

Current status (GA, Public preview, or Private preview).

- Status – Public preview. 

Incremental Refresh for Materialized Views on data lake tables

Amazon Redshift will now incrementally refresh materialized views created on Iceberg tables and standard AWS Glue tables. This eliminates full refreshes of the materialized views which require the re-execution of the SQL statements within the materialized view and re-writing the data contained in the materialized view.

Important things to know

- Materialized views provide a mechanism for precomputing the result set for complex queries involving large data sets and multiple table joins or aggregations.
- Incremental refreshes of materialized views have been available in most data warehouses for many years.

Current status (GA, Public preview, or Private preview).

- Status – Public preview. 

New Fine Grained Access Control (FGAC) to nested objects

Amazon Redshift can now apply fine grained access control (FGAC) to nested objects within the data lake. These nested objects include files in Parquet, ORC, JSON, and Ion file formats. AWS Lake Formation FGAC can now be applied to these objects, and they can be queried with Amazon Redshift data lake analytics. By using Dynamic Data Masking (DDM) within Amazon Redshift, masking policies can be applied to protect sensitive data.

Important things to know

- The new fine grained access control support requires the AWS Lake Formation (separately priced) service to provide the FGAC capability for Amazon Redshift nested object controls.

Current status (GA, Public preview, or Private preview).

- Status – Public preview. 

Competitive analysis 

The recent announcements around Amazon Redshift improve the overall data warehouse capabilities, but several of the features rely on additional AWS services that a client must purchase to utilize a new capability. In addition, capabilities like Multidimensional Data Layout (MDDL) are behind capabilities that IBM already delivers with Db2 Warehouse on Cloud. Db2 provides Multidimensional Clustering (MDC) tables to allow table data to be sorted by multiple table dimensions that is under total client control versus being controlled by database tooling. In addition, BLU acceleration (column-organized) tables utilize a synapse table and can optionally have additional indexes built on the table (with a tool to assist clients in choosing the table type and indexes to create) to ensure query performance versus depending solely on database tooling. 

From a broader data lakehouse perspective, IBM watsonx.data provides hybrid cloud data source support and deployment options for private cloud, public cloud, or traditional on-premises. To have the same range of capabilities, AWS clients must use the Amazon Athena, Amazon Redshift, and AWS Cloud Formation, while at the same time being limited to AWS only for data sources and deployment.  

As a final competitive point, a majority of the Amazon Redshift new capabilities are still only in preview and cannot be used in production environments (as of December 1st, 2023). 

**Data Lakehouse** 

Amazon Athena support for Amazon S3 Express One Zone storage

Amazon Athena now supports Amazon S3 Express One Zone storage to replace standard S3 with higher performance storage and AWS claims that Amazon Athena query performance improves by up to 2.1x over standard S3 storage. This will improve Amazon Athena’s performance and make it a stronger competitor in the data lakehouse market, especially for clients that are running their IT infrastructure on AWS. Amazon S3 Express One Zone utilizes a new directory bucket type, which is the biggest differentiator compared to regular S3 (regular buckets).

![](Aspose.Words.d0641802-ffd0-48e5-85aa-e6037c291563.007.jpeg)

*Figure 4 - An AWS provided diagram describing Amazon S3 Express One Zone storage.*

Important things to know

Although Amazon S3 Express One Zone storage is more performant, there are some drawbacks:  

- S3 Express One Zone storage is available in a single availability zone (no protection against region failure). 
- S3 Express One Zone storage cost is ~8x the cost of standard S3 storage (0.16 vs. 0.023 per GB per month).
- S3 Express One Zone is limited to four AWS data centers today: 
- U.S. East (N. Virginia) 
- U.S. West (Oregon) 
- Europe (Stockholm) 
- Asia Pacific (Tokyo) 

Current status (GA, Public preview, or Private preview).

- Status – General availability (GA). 

AWS Glue Data Catalog supports generating column-level statistics  

AWS Glue Data Catalog now supports generating column-level statistics for AWS Glue tables. These statistics are then integrated with the Cost Based Optimizer (CBO) from Amazon Athena and Amazon Redshift Spectrum resulting in improved performance and potential cost savings (based on queries using less compute resources). These statistics are column-level statistics such as number of distinct, number of nulls, max, and min on Parquet, ORC, JSON, ION, CSV, and XML file types. With statistics, analytics services such as Amazon Athena and Amazon Redshift can optimize queries by applying the most restrictive filters as early as possible during query processing. 

Important things to know

- A client must collect statistics for the AWS Glue tables, the column-level statistics are not populated automatically.

Current status (GA, Public preview, or Private preview).

- Status – General availability (GA). 

AWS Glue Data Catalog supports multi-engine views with AWS Analytics Engines 

AWS Glue Data Catalog supports the creation of views that support multiple analytics engines within AWS. SQL views can be created within AWS Glue Data Catalog and queried from SQL engines including Amazon Athena, Amazon Redshift, and Spark with Amazon Elastic Map Reduce (EMR).  

Rather than creating separate views for each engine for data that will be shared across multiple analytics engines, AWS Glue Data Catalog allows a single view to be created to allow users to query data without granting privileges on the underlying base tables. Access to the views is controlled by the AWS Lake Formation service using the same resources used to grant access and control other resources in the data lake.

Important things to know

- Clients must use the separately priced AWS Lake formation service to govern and control the multi-engine views created within AWS Glue Data Catalog. 
- To create views in the Data Catalog, clients must register the underlying Amazon S3 data locations of the reference tables within AWS Lake Formation. 

Current status (GA, Public preview, or Private preview).

- Status – General availability (GA). 

Competitive analysis 

Although S3 Express One Zone provides improved performance over standard S3, it is considerably more expensive and limits a client to only AWS as their data landscape. IBM watsonx.data provides more options as well as integration with an IBM Storage Fusion HCI (Hyperconverged Infrastructure) appliance which provides comparable or better performance to S3 Express One Zone without limiting a client to AWS for their data landscape, delivering a true hybrid cloud data environment.

The enhancements to AWS Glue Data Catalog strengthen the overall AWS data lakehouse solution but the primary competitive weakness of supporting a data lakehouse on a single cloud with no hybrid cloud capability still remains.

**SUMMARY ![](Aspose.Words.d0641802-ffd0-48e5-85aa-e6037c291563.008.png)**

AWS continues to advance their public cloud infrastructure and services every year and makes notable announcements at each re:Invent conference. However, AWS continues to offer solutions for data and AI that are limited to a single public cloud with no real solutions for clients that require a hybrid cloud environment to meet their complete data environment requirements. 

IBM watsonx provides a complete AI and Machine Learning (ML) platform that provides an open data lakehouse, Large Language Models (LLMs), traditional AI, and a governance solution that ensures trustworthy AI. In addition, watsonx is integrated into IBM’s Cloud Pak for Data (CP4D) hybrid cloud data fabric that provides deployment flexibility and integration with OEM services to provide a complete data platform for clients.
© 2023 IBM Corporation. For comments and questions, please contact Danny Arnold [(darnold@us.ibm.com)](mailto:darnold@us.ibm.com) 
