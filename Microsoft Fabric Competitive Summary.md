![ref1] ![ref2]

Competitive Information **Microsoft Fabric Update – Dec. 2023**

Microsoft Fabric Details 

Overview 

Microsoft Fabric is now general availability (as of November 2023) and this document highlights the main components and features of Microsoft Fabric (available in Microsoft Azure) along with competitive positioning against IBM watsonx.data as a data lakehouse. 

© 2023 IBM Corporation. For comments and questions, please contact Danny Arnold [(darnold@us.ibm.com)](mailto:darnold@us.ibm.com) For additional information, please see the[ Microsoft Fabric ](https://learn.microsoft.com/en-us/fabric/get-started/microsoft-fabric-overview)and[ Microsoft OneLake ](https://learn.microsoft.com/en-us/fabric/onelake/onelake-overview)documentation. 
![ref1] ![ref2]

Competitive Information **Microsoft Fabric Update – Dec. 2023**

Microsoft Fabric is an all-in-one analytics solution that provides a suite of services 

- Data Engineering  
- Data Factory 
- Data Science 
- Data Warehouse 
- Real-time Analytics 
- Power BI 

across the following components: 

© 2023 IBM Corporation. For comments and questions, please contact Danny Arnold [(darnold@us.ibm.com)](mailto:darnold@us.ibm.com) For additional information, please see the[ Microsoft Fabric ](https://learn.microsoft.com/en-us/fabric/get-started/microsoft-fabric-overview)and[ Microsoft OneLake ](https://learn.microsoft.com/en-us/fabric/onelake/onelake-overview)documentation. 
![ref1] ![ref2]

Competitive Information **Microsoft Fabric Update – Dec. 2023**

High-level Architecture 

Microsoft Fabric requires Microsoft OneLake for every Data Fabric installation and there can only be a single OneLake for each Microsoft Fabric tenant. OneLake provides the data lake service component of Microsoft Fabric with a single pane of glass filesystem namespace that spans across users, regions, and clouds. In addition to the proprietary compute engines shown on the diagram, Microsoft Fabric supports the proprietary Databricks Photon query engine along with open source Apache Spark.

![](Aspose.Words.8c939aaa-c9af-483e-a694-288eca041675.003.jpeg)

Figure 1 - Microsoft Fabric provides many services that access a single data lake (OneLake).

Microsoft OneLake 

Microsoft Fabric unifies OneLake and the data lakehouse architecture across enterprises. OneLake itself is built on top of Azure Data Lake Storage (ADLS) Gen 2 and is the native data store for Microsoft Fabric. OneLake provides a single Software as a Service (SaaS) experience and single tenant-wide data store that contains all data.

Within a single tenant, data can be divided into workspaces to provide separation of data to allow different access permissions and different data lakehouses to coexist within the single OneLake instance. A workspace can contain lakehouses, warehouses, data sets, and Kusto databases (native database structure within OneLake) to provide granularity within a client’s overall Microsoft Fabric environment. Each lakehouse, dataset, warehouse, or Kusto database is contained within a sub-folder that exists within a parent workspace folder.

NOTE: By Microsoft’s definition, a *lakehouse* is a collection of files, folders, and tables that represent a database over a data lake.

![](Aspose.Words.8c939aaa-c9af-483e-a694-288eca041675.004.jpeg)

Figure 2 - An example showing multiple folders within a OneLake instance.

Looking at OneLake in more detail, OneLake provides OneSecurity and provides the storage for warehouses, lakehouses, Kusto Query Language (KQL) databases (OneLake’s native SQL engine, listed as Kusto DB in the diagram), and datasets. 

![](Aspose.Words.8c939aaa-c9af-483e-a694-288eca041675.005.jpeg)

Figure 3 - Overview diagram of Microsoft Fabric including OneLake details.

OneLake stores all warehouses and lakehouses in Delta Lake open table format in Parquet files.

For data that is not contained in lakehouses or Kusto Query Language (KQL) databases, for example, an Amazon Simple Storage Service (S3) Delta-Parquet file in Amazon Web Services (AWS), OneLake provides shortcuts. Shortcuts define external data sources so that the data can be accessed by Microsoft Fabric components without having to move or copy data physically into either a OneLake lakehouse or Kusto Query Language (KQL) databases. Earlier in this document, the structure of folders within OneLake was discussed, where lakehouses, warehouses, datasets, and Kusto sub-folders can exist within an OneLake workspace. This folder structure is important to remember when defining shortcuts within OneLake. Within the lakehouse and Kusto Query Language (KQL) databases main folder, there exists two sub-folders, Tables and Files. In the Tables folder, only the top level of the folder is usable for defining data source shortcuts (there can be no subdirectory hierarchy within this directory). If a shortcut is defined in the Tables folder, it is automatically managed by OneLake. For example, a shortcut is defined on a S3 bucket in AWS containing multiple Delta-Parquet files to an OneLake lakehouse. Since this shortcut defines a supported OneLake table format (Delta Lake) and file format (Parquet), it is fully managed by OneLake. If a new Delta table (Delta-Parquet file) is added to this S3 bucket, that table would be automatically discovered by OneLake and would be available for access in the lakehouse. If a shortcut is defined on data that is not a supported format (for example, a S3 bucket containing Apache Iceberg Parquet files in AWS where a specific Iceberg table is defined to OneLake), this shortcut would be created in the Files folder. The Files folder is managed by the client and is allowed to have sub-directories and a hierarchical directory structure. The drawback to shortcuts in the Files folder is that each shortcut has to be defined explicitly by a client before that data object is accessible in OneLake using the Microsoft Fabric components.

![](Aspose.Words.8c939aaa-c9af-483e-a694-288eca041675.006.jpeg)

Figure 4 - Tables and Files directory structure within Microsoft OneLake

From a multi-cloud perspective, Microsoft Fabric and OneLake is not restricted to only Microsoft Azure,  as data sources can be defined to other OneLake locations (in different tenants), ADLS, Amazon S3 storage accounts, or Dataverse (a Microsoft scalable low-code data platform). However, the standard open table format in AWS (with the exception of AWS Databricks clients) is predominately Apache Iceberg (not Delta Lake), so these data sources must be manually configured and maintained by a client.

Microsoft OneLake Advantages 

According to Microsoft, Microsoft OneLake delivers these primary advantages to clients:

- One data lake for the entire organization.
- One copy of data for use with multiple analytical engines.

Competitive Analysis 

Microsoft Fabric and Microsoft OneLake provide a data fabric and data lakehouse solution for clients that primarily run on Microsoft Azure except for some Amazon S3 files on AWS. For clients that have a true hybrid cloud or multi-cloud environment (that is not limited Microsoft Azure and Amazon S3 files on AWS),  the combination of IBM Cloud Pak for Data (CP4D) and IBM watsonx.data provides a more flexible and robust data fabric and data lakehouse solution.

From a data lakehouse perspective, Microsoft Fabric and Microsoft OneLake have several disadvantages compared to IBM watsonx.data: 

- OneLake uses the Delta Lake open table format, which is open source software that is controlled by Databricks (a strategic Microsoft Azure partner) and the Azure Data Lake Storage (ADLS) component is also based on Delta Lake. Most of the other cloud providers (AWS and Google Cloud Platform (GCP)) support Delta Lake for their Databricks clients, but favor Apache Iceberg as their open table format for non-Databricks use. IBM watsonx.data uses Apache Iceberg as the open table format, allowing clients on other cloud providers (AWS and GCP) to utilize other query engines with their Iceberg tables. For example, any Iceberg tables that reside on AWS could use the watsonx.data Presto query engine that provides fixed compute configurations for consistent performance versus using an Amazon Athena serverless as the query engine. Additionally, watsonx.data extends the data lakehouse from a single cloud to the hybrid cloud.
- OneLake limits the choice of query engines to Microsoft Azure and AWS and the use of Delta Lake (Delta-Parquet) tables limits the query engines to Databricks (AWS and Microsoft Azure) and Microsoft Fabric Serverless compute options (Microsoft Azure). IBM watsonx.data allows any query engine that supports Apache Iceberg (as long as the metadata for those tables is shared) to be used as a query engine and includes Presto and Spark query engines with seamless integration for IBM clients that want to use Netezza Performance Server as a Service (NPSaaS) or Db2 Warehouse on Cloud (Db2 WoC) query engines for query workloads that require optimal performance today (with integration for on - premises NPS and Db2 coming in 2024).
- Each Microsoft Fabric tenant can have only one OneLake with lakehouses, warehouses, datasets, and KQL databases being separated into workspaces under that single OneLake instance. IBM watsonx.data provides flexibility by allowing a single data lakehouse for all data sources or multiple data lakehouses to easily separate and manage data based on applications, departments, or other categories providing flexibility to meet an individual client’s requirements. IBM Cloud Pak for Data and watsonx.data provide an open, flexible hybrid cloud solution that can adapt to a client’s changing requirements over time without locking them into a single cloud provider.

To specifically address Microsoft OneLake’s advantages when discussing watsonx.data in competitive sales situations: 

- One data lake for the entire organization – Microsoft OneLake provides a single data lake for the entire organization as long as all data sources that are part of the data lake reside in Microsoft Azure and Amazon S3 files on AWS. If an organization has other data that should be included within the data lake, OneLake cannot address a client’s data lakehouse requirements. By contrast, IBM watsonx.data fully supports hybrid cloud and can satisfy the one data lakehouse for an entire organization requirement by allowing on-premises data sources such as Teradata and SAP HANA and cloud data sources outside of Amazon S3 files and Microsoft Azure such as Snowflake on Google Cloud Platform, or data on other clouds. 
- One copy of the data for use by multiple analytical engines – Microsoft OneLake allows query engines owned by Microsoft or Databricks on Microsoft Azure to access OneLake data. IBM watsonx.data supports multiple analytical engines to access data lakehouse data as well, with Presto, Apache Spark, Db2, and Netezza Performance Server engines available as well as any query engine that supports Iceberg tables. The default SQL query engine provided by OneLake in Microsoft Azure is Kusto Query Language (KQL), which is only used on Microsoft Azure. IBM watsonx.data within IBM Cloud and AWS provides the Presto query engine which is widely adopted outside of watsonx.data and is used by Meta, Netflix, and other organizations to perform analysis on very large data sets (exabyte scale, over 1 billion gigabytes).  

Summary 

Microsoft Fabric with Microsoft OneLake provides a data fabric and data lakehouse environment in Microsoft Azure. However, it has limitations due to Microsoft’s adoption of the Delta Lake open table format (controlled by Databricks) and the limited support for data sources outside of Microsoft Azure. 

One of the primary reasons that clients are interested in a data lakehouse compared to the older date warehouse centric configurations is the ability to incorporate many different data sources in different locations to allow access to all data without having to copy or duplicate data. Limiting a data lakehouse solution to primarily a single cloud vendor (Microsoft Azure) seems to eliminate one of the perceived benefits of selecting a data lakehouse solution.

Although Microsoft Fabric and Microsoft OneLake use the open source Delta Lake open table format, it was developed by Databricks and is primarily under the control of Databricks. Contrast this with the open source Apache Iceberg open table format, which has been adopted by IBM watsonx.data, Amazon Athena, Amazon Redshift, Snowflake, Dremio, Starburst, and other vendors and has a broad community of contributors that fosters a more open approach to new capabilities as Apache Iceberg development moves forward. By comparison, Delta Lake is used by Databricks and Microsoft Azure, with no real contributors other than Databricks. 

From a SQL query engine perspective, Microsoft Fabric with Microsoft OneLake provides the Azure Analytics (proprietary) query engines (for example, Azure Synapse Analytics data warehouse) and the Databricks Photon (proprietary) SQL query engine with Apache Spark the only open source query engine supported. IBM watsonx.data provides the open source Presto SQL query engine along with Apache Spark. With Microsoft Fabric and Microsoft OneLake, the focus is to only use query engines from Databricks (strategic Microsoft Azure partner) and Microsoft Azure. IBM watsonx.data clients can use any query engine that supports Apache Iceberg and has access to the metadata catalog in the hybrid cloud providing flexibility for clients.

Microsoft’s stated advantages for Microsoft OneLake does not differentiate OneLake from watsonx.data: 

- A single data lakehouse for an entire organization.
- One copy of the data for use by multiple analytical engines.

IBM watsonx.data has the advantage of a larger data landscape supported by the lakehouse, as watsonx.data fully supports the hybrid cloud to ensure clients are not limited by where their data resides. Unless a client is content to limit their lakehouse to Microsoft Azure and AWS, IBM watsonx.data provides a more complete lakehouse solution.

For potential clients that are looking to adopt a data fabric and data lakehouse technology, there are several advantages to choosing IBM Cloud Pak for Data with watsonx.data over Microsoft Fabric with Microsoft OneLake:

- More open Apache Iceberg open table format that is supported by many organizations that use the technology (Meta, Netflix, and others) and a community of contributors versus open source software controlled by a single vendor (Delta Lake by Databricks). 
- An open source SQL query engine with Presto in watsonx.data versus the proprietary SQL query engines in Microsoft Fabric and Databricks. 
- Hybrid cloud data sources and hybrid cloud deployment options are supported by watsonx.data versus the single cloud (Microsoft Azure) and Amazon S3 files on AWS support of Microsoft Fabric and Microsoft OneLake.
© 2023 IBM Corporation. For comments and questions, please contact Danny Arnold [(darnold@us.ibm.com)](mailto:darnold@us.ibm.com) For additional information, please see the[ Microsoft Fabric ](https://learn.microsoft.com/en-us/fabric/get-started/microsoft-fabric-overview)and[ Microsoft OneLake ](https://learn.microsoft.com/en-us/fabric/onelake/onelake-overview)documentation. 

[ref1]: Aspose.Words.8c939aaa-c9af-483e-a694-288eca041675.001.png
[ref2]: Aspose.Words.8c939aaa-c9af-483e-a694-288eca041675.002.png
