**Evaluation Warning : The document was created with Spire.Presentation for Python**whats new?![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.001.jpeg)

V1.1.0-29 Nov

Watsonx.data

PM team watsonx.data![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.002.png)![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.003.png)

**Evaluation Warning : The document was created with Spire.Presentation for Python**Seller guidance  Slides in this presentation marked as  References in this presentation to IBM and legal disclaimer **"IBMOnly**use and should not be shared with " are for IBM and Business Partner **and Business PartnerInternal Use**  imply that they will be available in all countries in which IBM operates. Product release dates and/or 

products, programs, or services do not clients or anyone else outside of IBM or ![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.004.png)![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.005.png)

the Business Partners’ company. capabilities referenced in this 

presentation may change at any time at 

© IBM Corporation 2023.  IBM’s sole discretion based on market **All Rights Reserved.** opportunities or other factors and are 

not intended to be a commitment to 

The information contained in this  future product or feature availability in publication is provided for informational  any way. Nothing contained in these purposes only. While efforts were made  materials is intended to, nor shall have 

to verify the completeness and accuracy  the effect of, stating or implying that any 

of the information contained in this  activities undertaken by you will result in IBM and Business Partner  publication, it is provided AS IS without  any specific sales, revenue growth, or 

Internal Use Only warranty of any kind, express or implied.  other results. 

In addition, this information is based on 

IBM’s current product plans and strategy,  All client examples described are 

which are subject to change by IBM  presented as illustrations of how those without notice. IBM shall not be  clients have used IBM products and the responsible for any damages arising out  results, they may have achieved. Actual of the use of, or otherwise related to,  environmental costs and performance this publication or any other materials.  characteristics may vary by client. Nothing contained in this publication is 

intended to, nor shall have the effect of, 

creating any warranties or 

representations from IBM or its 

suppliers or licensors, or altering the 

terms and conditions of the applicable 

license agreement governing the use of 

IBM software.

**Evaluation Warning : The document was created with Spire.Presentation for Python** 

Agenda ![ref1]

- Overview

**Key take aways**

- Register Spark

Additional features,  fixes, and enhancements are being 

- Db2+NZ engine registrations

delivered in every release. 

- New Connectors

These will be shared:  • Bucket enhancements

- in periodic enablement like this, posted to the saleskit:  • IBM Knowledge Catalog (IKC) Integration <https://ibm.biz/watsonx-data-saleskit> • Additional Enhancements
- in documentation [for both SW and](https://www.ibm.com/docs/en/watsonxdata/1.0.x?topic=watsonxdata-release-notes) for [Cloud  ](https://cloud.ibm.com/docs/watsonxdata?topic=watsonxdata-release)• Private Preview Features Highlights
  - Prestissimo
  - Milvus DB
  - Optimizer+
  - Semantic Automation

• Call to Action
**Evaluation Warning : The document was created with Spire.Presentation for Python**

Overview![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.007.png)



**Evaluation Warning : The document was created with Spire.Presentation for Python**Overview of the key components of the IBM watsonx.data: multiple query engines, open 

table formats and built-in enterprise governance
**

**



**Your existing  ![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.008.png)![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.009.png)![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.010.png)**

**ecosystem** Data warehouse Data lake

5 **Multiple engines** such as Presto and Spark that **Query engines** provide **fast, reliable, and efficient processing ![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.011.png)![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.012.png)**

**of big data** at scale

**Governance  Built-in governance** that is compatible with **and Metadata Metadata store** existing solutions such as watsonx.governance 

**Access control management** and IBM Watson Knowledge Catalog

**Vendor agnostic open formats** for analytic data ![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.013.png)![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.014.png)**Data format** sets, allowing different engines to access and ![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.015.png)![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.016.png)![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.017.png)

share the same data, at the same time

**Cost effective, simple object storage** available **Storage** across hybrid-cloud and multi-cloud ![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.018.png)![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.019.png)![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.020.png)![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.021.png)

![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.022.png) ![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.023.png) environments

**Hybrid-cloud deployments** and workload **Infrastructure** portability across hyperscalers and on-prem ![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.024.png)![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.025.png)![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.026.png)![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.027.png)![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.028.png)

with Red Hat OpenShift

watsonx.data 

IBM Software | © 2023 IBM Corporation | Confidential

Core watsonx.data functionality Ecosystem infrastructure

**Optimize workload costs and performance ![ref2]![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.030.png)using multi-engine functionality** 

**Ensure governance and reduce time ![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.031.png)to insight with centralized metadata and access management**

**Access all of your data across databases ![ref2]and data lakes**

**Reduce storage costs and facilitate ![ref2]data ingest** 

**Deploy on any infrastructure and ![ref2]optimize available resources**

**Evaluation Warning : The document was created with Spire.Presentation for Python**Access all your data, quickly and optimize your data architecture with multi-engine support 

and hybrid deployment of analytics and AI workloads 



|<p>1</p><p>![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.032.png)</p><p>**Cloud warehouse**</p>|<p>3</p><p>![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.033.png)</p><p>**Cloud data lake**</p>|
| - | - |
|**IBM wats**|**onx.data**|
|<p>![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.034.png)</p><p>**On prem warehouses**</p><p>2</p>|<p>![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.035.png)</p><p>**On prem lakes**</p><p>4</p>|

1![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.036.png)![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.037.png)![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.038.png)

**Optimize costly cloud warehouses** Make the most of fit-for-purpose query  engines and compute resources  

2

**Optimize and access on-prem warehouses** Use low-cost object storage and fit-for- purpose engines

3 4

**Modernize data lakes** 

Run existing reporting and enable new AI workloads without the cost and complexity of Hadoop. 

1 2 3 4

**Deploy across hybrid cloud and multicloud** Seamlessly deploy to both the public cloud and to your existing on-premises investment

Types of workloads

Structured Unstructured Technology

Proprietary Open

IBM Software | © 2023 IBM Corporation | Confidential 6

**Evaluation Warning : The document was created with Spire.Presentation for Python** 

Access all your data through  ![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.039.png)![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.040.png)

a single point of entry across  **watsonx.data** 

all clouds and on-premises  environments 

Scale AI workloads, 

for all your data, anywhere Get started in minutes with built-in governance, security, and automation 

A fit-for-purpose data store, based on an open  ![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.041.png)lakehouse architecture, supported by querying,  governance and open data formats to access  and share data.  

*Available as a service on IBM Cloud and AWS as a managed  ![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.042.png)*

*service, and software-as-a-container* Reduce the cost of your data  

warehouse by up to 50%\*  through workload optimization  across multiple query engines  and storage tiers.  

IBM Briefing / Gartner MQ for CDMS 2023 / © 2023 IBM Corporation 7

**Evaluation Warning : The document was created with Spire.Presentation for Python** 

Agenda ![ref1]

- Overview
- Register Spark
- Db2+NZ engine registrations
- New Connectors
- Bucket enhancements
- IBM Knowledge Catalog (IKC) Integration
- Additional Enhancements
- Private Preview Features Highlights
  - Prestissimo
  - Milvus DB
  - Optimizer+
  - Semantic Automation

• Call to Action
**Evaluation Warning : The document was created with Spire.Presentation for Python Key Takeaways**

Spark Engine • Spark can now be used with watsonx.data![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.043.png)![ref3]

- Leverage Spark for ingest and transformations

**Why:** • Use EMR Spark with watsonx.data in AWS deployments A customer may want to leverage Spark for ingestion, data transformation, and iceberg table maintenance. A customer may also choose to use Spark for other purposes given its  • Configure  open-source Spark to work with watsonx.data

broad applicability.  ![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.045.png)

**How:** 

- *On Software:* 
  - Customers can **provision** a Spark engine *with their entitlement of  watsonx.data and then proceed to register it* 
  - Customers can **register** an existing IAE Spark engine 
  - Customers can **configure** open-source Spark to work with watsonx.data  using watsonx.data documentation 
- *On IBM Cloud SaaS:* 
  - Customers can **register** an existing Spark engine service on IBM Cloud 
  - Customers can **configure** open-source Spark to work with watsonx.data  using watsonx.data documentation 
  - Customers **cannot provision** a Spark engine in watsonx.data on IBM Cloud 
- *On AWS SaaS:* 
  - Customers can **configure** AWS EMR to work with watsonx.data using  watsonx.data documentation ![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.046.png)
  - Customers can **configure** open-source Spark to work with watsonx.data  using watsonx.data documentation 
  - Customers **cannot provision** a Spark engine within watsonx.data on AWS 
- Customers can run bulk ingestion jobs using the Spark instance that is provisioned or  registered via UI or CLI 

**Provision:** Customers create a Spark engine. 

**Register:** Customers provide Spark engine details to connect watsonx.data to Spark engine. **Configure:** Customers connect to watsonx.data using watsonx.data documentation. 


**Evaluation Warning : The document was created with Spire.Presentation for Python Key Takeaways**

Db2+NZ engine registrations • Db2 and Netezza can now be registered with and ![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.047.png)![ref3]

appear in the UI of watsonx.data

**Why:**A customer may want to see the Db2 and/or NZ data  ![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.048.png)warehouse engine that they are using to work with iceberg tables  that are held in the watsonx.data metastore. 

**How:** 

- Register the engine with valid console url 
- on registering, check the engine detail page to view the  console url, metastore url, and the bucket which can be used  in the engine 
- On clicking the console link, console login page is opened. 
- Login, register the bucket(s) and the metastore. 
- The table from the catalog can be seen in the mapped DB 

**Limitations**: ![](Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.049.png)

- Cannot run queries from within watsonx.data- must do so in  Db2 or NZ 
- For configuration must manually gather and input  configurationdetails per guidance in docs 

[ref1]: Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.006.png
[ref2]: Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.029.png
[ref3]: Aspose.Words.1bf097be-6c56-4e1d-a08d-3839ac250e98.044.jpeg
