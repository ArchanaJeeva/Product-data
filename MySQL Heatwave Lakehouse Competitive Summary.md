![](Aspose.Words.7e736fe1-695b-474e-babd-b9f1061bca77.001.png) ![](Aspose.Words.7e736fe1-695b-474e-babd-b9f1061bca77.002.png)

Competitive Information

**TECHNICAL INFORMATION AND PRELIMINARY ANALYSIS** ![](Aspose.Words.7e736fe1-695b-474e-babd-b9f1061bca77.003.png)

Oracle has recently announced MySQL HeatWave Lakehouse and has distributed some technical information about this new offering as well as benchmark comparisons against other vendors. Although the product name includes “Lakehouse”, it is important to understand the MySQL HeatWave Lakehouse offering and how it differs from true lakehouse offerings like IBM watsonx.data. With a product name that begins with “MySQL”, a common assumption would be that this offering is open source. However, that would be a false assumption as MySQL HeatWave Lakehouse is not available as part of open source MySQL and is an Oracle proprietary offering that is available only on the public cloud as a fully managed offering. 

Oracle’s MySQL HeatWave Lakehouse is only available on Oracle Cloud Infrastructure (OCI) and Amazon Web Services (AWS), with full functionality on AWS with the OCI still ramping up to full capabilities. This document will provide some technical details and a high-level competitive analysis to assist sellers in positioning IBM watsonx.data correctly against MySQL HeatWave Lakehouse 

MySQL HeatWave Lakehouse details

MySQL HeatWave Lakehouse (LH) is a new offering from Oracle and provides a fully managed lakehouse offering that is available on AWS and OCI. Oracle provides a white paper that provides a technical overview of MySQL HeatWave LH at this URL. 

MySQL HeatWave Lakehouse is trying to solve the data problem experienced by many organizations today where data analysis needs to address data sources that are outside of a traditional data warehouse and data processing needs to be performed on the entire data landscape (all data sources) without movement or duplication of the external data into the data warehouse.

Oracle has released MySQL HeatWave LH to address this data challenge by allowing MySQL HeatWave LH to access data outside of MySQL (and its InnoDB storage engine) by allowing direct processing of data contained in object store using open file formats such as Apache Parquet, Comma Separated Values (CSV), and a limited set of data sources. For example, data contained in Amazon Redshift, Amazon Aurora, Oracle Database, and MySQL export files can be processed directly by MySQL HeatWave Lakehouse. 

![](Aspose.Words.7e736fe1-695b-474e-babd-b9f1061bca77.004.jpeg)

*Figure 1 - MySQL HeatWave Lakehouse architecture* 

To allow processing against data volumes up to 0.5 petabyte (500 TB), MySQL HeatWave LH allows database clusters of up to 512 nodes to be used in parallel.

Oracle publishes some bold performance claims in their white paper about MySQL HeatWave LH

![](Aspose.Words.7e736fe1-695b-474e-babd-b9f1061bca77.005.png)

It should be noted that this TPC-H benchmark result is NOT published on the Transaction Processing Council (TPC) website as an official, certified benchmark result. The actual scripts and other benchmark details are provided on GitHub at this URL. Oracle[ ](https://github.com/oracle/heatwave-tpch)does provide this statement about the TPC-H benchmark results:

“Benchmark queries are derived from the TPC-H benchmark, but results aren’t comparable to published TPC-H benchmark results since these don’t comply with the TPC-H specification.” 

The published benchmark results are shown in the table below and a write-up is available here. 

![](Aspose.Words.7e736fe1-695b-474e-babd-b9f1061bca77.006.jpeg)

Another fact to consider is that the MySQL HeatWave LH cluster for the 500 TB benchmark used 512 MySQL HeatWave LH nodes, which is the maximum data volume and configuration possible. The MySQL HeatWave LH 512 node configuration performance was compared to a 4X-Large (4XL) Snowflake configuration (128 servers), a 20 ra3.16xlarge Amazon Redshift nodes, 6,400 query slots on Google BigQuery, and a 3X-Large Databricks system on AWS. This seems to indicate that MySQL HeatWave LH had more compute horsepower than the other competitors used in the benchmark comparison. In addition, these other data warehouse solutions have room to grow to larger configurations than possible with MySQL HeatWave LH.  

The **total annual cost for the 512 node fully managed MySQL HeatWave LH solution is $1,742,036** which is not exactly an inexpensive data lakehouse solution and this is the maximum configuration and data volume that MySQL HeatWave LH supports. Clients using other data lakehouse solutions are not limited to 500 TB of data, and large data volumes are the primary reason that clients are considering data lakehouse solutions.

**Status** –  General availability announced on July 20, 2023.

Competitive analysis 

There are several competitive differentiators where IBM watsonx.data has an advantage over MySQL HeatWave LH. Here are the main differentiators to highlight with clients:

- MySQL HeatWave LH does not utilize an open table format (Apache Iceberg, Delta Lake, or Hudi), so the data accessed by MySQL HeatWave LH cannot be accessed by an open source query engine like Presto or Apache Spark. This means clients are restricted to using the MySQL HeatWave LH query engine and are locked into the two clouds where Oracle offers MySQL HeatWave LH; AWS and OCI. 
- MySQL HeatWave LH is not an open source solution despite MySQL being part of the name. MySQL Heatwave LH has proprietary Oracle internals and is NOT available outside of the two public cloud solutions on AWS and OCI. 
- MySQL HeatWave LH is limited multi-cloud, but not hybrid cloud providing an advantage for IBM watsonx.data for clients whose data and workloads are not restricted to AWS and OCI. IBM watsonx.data provides a flexible lakehouse solution that incorporates open source components to ensure clients are not locked into a proprietary, niche solution.
- MySQL HeatWave LH uses a unified query engine that transforms all data sources into a unique, highly optimized internal format. The query engine behind MySQL HeatWave LH is not an open source engine and all development of the MySQL HeatWave LH offering is controlled and managed by Oracle. 

There is NO hybrid cloud solution available for MySQL HeatWave LH either from either a deployment or data source perspective (outside of Oracle Database and MySQL export files, which are both controlled by Oracle). The other data sources (outside of open file formats such as Apache Parquet and CSV) are data sources within AWS, which has partnered with Oracle as a deployment cloud for MySQL HeatWave LH.

**SUMMARY ![](Aspose.Words.7e736fe1-695b-474e-babd-b9f1061bca77.007.png)**

MySQL HeatWave Lakehouse (LH) is a proprietary, limited public cloud solution (AWS and OCI only) whose differentiating feature is that it can handle open file formats (Apache Parquet, CSV, and others) and limited export files from databases owned by Oracle Corporation and AWS (their hyperscaler partner in this solution) with Oracle Database, MySQL, Amazon Aurora, and Amazon Redshift support.

MySQL HeatWave LH 500 TB TPC-H benchmark results are not official and are NOT certified by the Transaction Processing Council. The benchmark was configured to highlight MySQL HeatWave LH and it is not specified what conditions and tuning configurations were used for the other vendors in the benchmark comparison (it was stated that the other vendor performance numbers were provided by a third party).

IBM watsonx.data provides an open source based data lakehouse solution that does not lock a client into one vendor’s proprietary technology and uses the Apache Iceberg open table format to allow flexibility of compute engines used for query processing versus the single compute engine of MySQL HeatWave LH. 

For clients that require a hybrid data lakehouse environment, IBM watsonx.data can be deployed on both hyperscaler (AWS, Microsoft Azure, and GCP) and other public clouds as well as private clouds and on-premises environments. Data sources can be distributed across the data lakehouse environment and accessed directly as Apache Iceberg tables or using connectors for external data sources across a wide variety of data sources. In contrast, MySQL HeatWave LH can access data sources in cloud object storage (on AWS and OCI) and export files for MySQL, Oracle Database, Amazon Aurora, and Amazon Redshift, which is a very limited set of data sources for a data lakehouse.

Oracle seems to be focused with MySQL HeatWave LH on overall performance versus competitors without providing any alternative methods of cost optimization (for example, different query engines) and uses the maximum MySQL HeatWave LH data volume (500 TB) and configuration (512 nodes) to make their performance claims. This solution costs $1,742,036, which would not be considered a low-cost solution by most clients seeking a data lakehouse solution. With IBM watsonx.data, clients can start out with a small configuration and grow as their data volume and performance requirements change. With MySQL HeatWave LH, clients have no idea how a small system behaves or whether it is cost-effective compared to other solutions. All they know from Oracle’s recent benchmark figures is that the chosen MySQL HeatWave LH system (which is at maximum data capacity and size) supposedly loads and queries data faster than a set of competitors that are running smaller compute configurations which still have the capacity to grow and handle additional data volumes.
© 2023 IBM Corporation  For comments and questions, please contact Danny Arnold (darnold@us.ibm.com)
