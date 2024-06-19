![](Aspose.Words.e2a024e3-bd10-47fe-a3dd-fd3c58d4c8c1.001.png) ![](Aspose.Words.e2a024e3-bd10-47fe-a3dd-fd3c58d4c8c1.002.png)

Competitive Information **Iceberg Support Update – September 2023**

**INDIVIDUAL ANNOUNCEMENTS AND PRELIMINARY ANALYSIS** ![](Aspose.Words.e2a024e3-bd10-47fe-a3dd-fd3c58d4c8c1.003.png)

One of the announcements that Snowflake made as part of their Snowflake Summit conference in June 2023 was around managed Iceberg Tables. That initial information was based on capabilities in private preview (not available to the public) and not many details were provided. A recap of the Iceberg table support that was discussed at that point-in-time is below. Snowflake has recently provided more details about their Iceberg table support and this document provides an update on Snowflake Iceberg table support. 

Managed Iceberg Tables (older June 2023 information)

Prior to 2022, Snowflake only supported Apache Iceberg tables as read-only external tables, which do not perform as well as standard Snowflake tables. At Snowflake Summit 2022 (a year ago), Snowflake announced support for Apache Iceberg that allowed Snowflake to access Iceberg tables as another Snowflake table while clients benefited from using the Snowflake high - performance query engine for compute. Since Iceberg tables were now treated as Snowflake native tables, all table activity (insert, update, delete, and select) was allowed. However, these tables were not managed by Snowflake and required the Iceberg metadata to be kept updated using a separate catalog (versus the native Snowflake catalog). With the recent Snowflake Summit 2023 announcement, Snowflake now offers managed Iceberg tables, a “managed” Iceberg table includes Snowflake updating the Iceberg catalog as required, providing a complete Iceberg table solution (no need for separate Iceberg catalog maintenance).

Updated (current) information on Snowflake Iceberg table support

Native and external table support for Iceberg tables have now been merged into a single Snowflake table type. For metadata management of an Iceberg table, the client can choose to have the Iceberg table entirely managed by Snowflake or to use an external catalog for management of the Iceberg table. Snowflake is working on integration with other catalogs to make management of Iceberg tables easier for clients and initial external catalog integration has been done for Amazon Web Services (AWS) Glue Catalog. Snowflake is also adding a simple, low-cost method to convert an Iceberg table’s catalog from external to Snowflake internal making it easier for clients to onboard to Snowflake without re-writing entire tables. 

Further details 

Snowflake now provides these methods for handling Iceberg tables versus the old External Table: 

- Snowflake can serve as the table catalog for managing Iceberg tables. Using this mode, Snowflake can read and write Iceberg and Parquet data to your storage account, and Snowflake takes care of storage maintenance operations like compaction, expiring snapshots, and deleting orphan files. Iceberg Tables in this mode can either be created from scratch using methods such as CTAS or CREATE TABLE, or they can be created by converting an Iceberg Table previously created using an external catalog, without any underlying data rewrite or ingestion cost. 
- Snowflake can access Iceberg tables that are managed by an external (to Snowflake) catalog. Using this mode, Iceberg tables can also be easily integrated with external catalogs to very quickly and easily query Iceberg data sets from Snowflake. With an external catalog, Snowflake has read-only access to Iceberg data sets in your storage account, and the external catalog manages storage maintenance—or the client can manage the storage manually. At this point-in-time (during the private preview period), a client can either point Snowflake to a metadata file location or create a simple Catalog Integration with AWS Glue Catalog. A Catalog Integration is a new type of object in Snowflake that greatly simplifies metadata refresh in comparison to the previous Snowflake Iceberg offering with External Tables.  The diagram below describes the “catalog integration” object. 

  ![](Aspose.Words.e2a024e3-bd10-47fe-a3dd-fd3c58d4c8c1.004.jpeg)

At the present time, Snowflake has added an ALTER TABLE command that makes it simple to convert an externally managed Iceberg table to a Snowflake-managed Iceberg table. Without rewriting or reformatting any files in the storage bucket associated with the Iceberg table, catalog ownership changes from the external catalog to Snowflake. Over time, as Snowflake’s engine performs more write operations on the table such as INSERT, UPDATE, DELETE and MERGE, performance will continue to improve. 

Either of these new methods for configuring Iceberg tables for use with Snowflake provides better performance than the old External Table method of dealing with Iceberg tables. This is due to Snowflake using a specialized Parquet file scanner that utilizes catalog statistics from an Iceberg external catalog (~2x better performance than External Tables) or the native Snowflake catalog (significantly better performance). The performance differences are highlighted in this graph:

![](Aspose.Words.e2a024e3-bd10-47fe-a3dd-fd3c58d4c8c1.005.jpeg)Snowflake explains the performance gap between externally managed Iceberg and Snowflake managed Iceberg as the result of external processes being able to write to the external catalog but may not write full statistics information.

- **Status** – Private preview (no date specified for public preview period).

Competitive analysis 

Snowflake is positioning Iceberg table usage with Snowflake to use the Snowflake catalog for management purposes versus an external Iceberg catalog by providing the best performance with Snowflake managed Iceberg tables. Clients that use a Snowflake managed Iceberg table environment will no longer be able to use external query engines outside of the Snowflake data warehouse engine, which will eliminate compute cost-optimization capabilities for clients.

IBM watsonx.data does not lock clients into proprietary query engines by using a proprietary catalog. For flexibility and cost optimization capabilities, watsonx.data is a better choice than Snowflake as a data lakehouse environment. Combined with the lack of hybrid cloud deployment options and limited ability to use on-premises data sources, Snowflake is still a weak contender in the data lakehouse market for clients looking for cost-optimization and deployment flexibility.

**SUMMARY ![](Aspose.Words.e2a024e3-bd10-47fe-a3dd-fd3c58d4c8c1.006.png)**

This updated information from Snowflake around Apache Iceberg table support has streamlined the Snowflake approach to processing Iceberg tables. However, the management of Iceberg tables by the Snowflake catalog will severely limit the future flexibility and ability of clients to efficiently and cost-effectively process their Iceberg table data with other query engines.

Snowflake has improved processing performance of Iceberg tables significantly over their initial External Table only support, but limits a client’s flexibility by limiting the Iceberg metadata catalog choice to either Snowflake’s internal catalog or AWS Glue Catalog at the present time. Clients using Snowflake on Microsoft Azure or Google Cloud Platform are currently restricted to either using External Table support for Iceberg tables with Snowflake (poor performance and read-only access) or implementing the Snowflake internal catalog for Iceberg table management limiting the query engine to Snowflake.
© 2023 IBM Corporation. For comments and questions, please contact Danny Arnold [(darnold@us.ibm.com)](mailto:darnold@us.ibm.com) Snowflake information reference blog -[ https://www.snowflake.com/blog/unifying-iceberg-tables/ ](https://www.snowflake.com/blog/unifying-iceberg-tables/)
