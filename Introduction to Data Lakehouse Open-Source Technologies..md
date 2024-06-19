**Evaluation Warning : The document was created with Spire.Presentation for Python** 

Introduction to  ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.001.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.002.png)Data Lakehouse Open-Source  Technologies 

Kelly Schlamb 

WW Technology Sales Enablement kschlamb@ca.ibm.com 

**Evaluation Warning : The document was created with Spire.Presentation for Python![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.003.png)**

IBM **watsonx.data** – the next generation data lakehouse

**Your existing  ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.004.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.005.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.006.png)**

**ecosystem** Data warehouse Data lake

**Multiple engines** including Presto and Spark ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.007.png)Completely open. **Query engines** that provide **fast, reliable, and efficient ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.008.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.009.png)**

**processing of big data** at scale

No lock-in!

**Governance  Built-in governance** that is compatible with ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.010.png)**and Metadata Metadata store** existing solutions such as watsonx.governance 

**Access control management** and IBM Knowledge Catalog

Built on a  **Vendor agnostic open formats** for analytic data ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.011.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.012.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.013.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.014.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.015.png)**Data format** sets, allowing different engines to access and 

foundation of  share the same data, at the same time industry-embraced  **Storage Cost**available across hybrid-cloud and**effective, simple object storage![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.016.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.017.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.018.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.019.png)**

open-source  ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.020.png) ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.021.png) multicloud environments technologies. **Infrastructure Hybrid-cloud**portability across hyperscalers and on-prem **deployments** and workload ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.022.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.023.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.024.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.025.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.026.png)

with Red Hat OpenShift

watsonx.data  ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.027.png) Core watsonx.data functionality

![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.028.png) Ecosystem infrastructure

Let’s get familiar with some common open-source technologies used in watsonx.data and

data lakehouse architectures in general…

Storage,![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.029.png)

data file formats, and table formats

What is object storage?

**Object storage:![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.030.jpeg)**

- Low cost 
- Near unlimited scalability
- Extreme durability & reliability (99.999999999%)
- High throughput
- High latency (but can be compensated for)
- Basic units are *objects*, which are organized in *buckets*

![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.031.png)

- Most notable provider for object storage is Amazon S3 (Simple Storage Service) ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.032.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.033.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.034.png)
- Other vendors offer S3-compatible object storage ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.035.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.036.png)

The rise of cloud object storage for data lakes and lakehouses

Cloud object storage technology is displacing HDFS as de facto storage technology for data lakes



||**Object Storage**|**HDFS**|**Object Storage vs. HDFS**|
| :- | - | - | :- |
|**Elasticity**|Yes (decoupled)|No|S3 is more elastic|
|**Cost/TB/Month**|$23|$206|10X|
|**Performance**|20MB/s/core|90MB/s/core|2x better price/perf|
|**Availability**|99\.99%|99\.9% (estimated)|10X|
|**Durability**|99\.999999999%|99\.9999% (estimated)|10X+|
|<p>**Transactional** </p><p>**writes**</p>|Most technologies now provide strong consistency|Yes|Comparable|

![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.037.png)

![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.038.png)

![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.039.png)

Common data  ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.040.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.041.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.042.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.043.png)

file formats • Human-readable text • Human-readable text

- Each row corresponds • Open file and data to a single data record interchange format

Computer systems and  • Each record consists • Consists of attribute- applications store data of one or more fields,  value pairs and arrays in files delimited by commas • JSON = JavaScript

Object Notation

Data can be stored in  binary or text format 

File formats can ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.044.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.045.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.046.png)

be open or closed  • Open-source • Open-source • Open-source (proprietary/lock-in) • Binary columnar storage • Binary columnar storage • Row-oriented data 

- Designed for efficient  • Designed and optimized  format and serialization 

Open formats (Parquet,  data storage and for Hive data framework

ORC, and Avro) are  fast retrieval • Self-describing • Robust support for commonly used in data  • Highly compressible • Similar in concept schema evolution lakes and lakehouses • Self-describing to Parquet • Mix of text/binary

Apache Parquet ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.047.png)

Parquet is designed to support fast data processing **Row-oriented storage ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.048.png)**for complex data ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.049.png)

- Open-source 
- Columnar storage 
- Highly compressible with configurable compression **Column-oriented storage** options and extendable encoding schemas by data type ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.050.png)
- Self-describing: schema and structure metadata is included 
- Schema evolution with support for automatic schema merging 

Why do these things matter in a lakehouse?

- Performance of queries directly impacted by size and amount of file(s) being read
- Ability to read/write data to an open format from multiple runtime engines enables collaboration
- Size of data stored, amount of data scanned, and amount of data transported affect the charges incurred in using a lakehouse (depending on the pricing model)

Apache ORC ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.051.png)

- Open-source, **columnar storage** format ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.052.png)

**Column-oriented storage**

- Similar in concept to Parquet, but different design ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.053.png)![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.054.png)
- Parquet considered to be more widely used than ORC **Row-oriented storage**
- Highly compressible, with multiple compression options ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.055.png)
  - Considered to have higher compression rates than Parquet 
- Self-describing and type-aware
- Support for schema evolution
- Built-in indexes to enable skipping of data not relevant to a query
- Excellent performance for read-heavy workloads
  - ORC generally better for workloads involving frequent updates or appends
  - Parquet generally better for write-once, read-many analytics

Apache Avro ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.056.png)

- Open-source, **row-based** storage and serialization format
  - Can be used for file storage or message passing
- Beneficial for write-intensive workloads ![](Aspose.Words.8da5a4a0-7c6b-46e4-a897-e5a43c36a061.057.jpeg)
- Format contains a mix of text and binary 
  - Data definition: Text-based JSON 
  - Data blocks: Binary 
- Robust support for schema evolution 
  - Handles missing/added/changed fields 
- Language-neutral data serialization 
  - APIs included for Java, Python, Ruby, C, C++, and more
