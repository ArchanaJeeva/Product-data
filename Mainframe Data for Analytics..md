**Evaluation Warning : The document was created with Spire.Presentation for Python** 

**watsonx.data![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.001.jpeg)![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.002.jpeg)**

Mainframe Data for AI – Analytics Sales Play

Seller presentation

Anson Kokkat 

[ansonk@ibm.com ](mailto:ansonk@ibm.com)

WW Principal Product Manager, watsonx.data

Rohan Pednekar [Rohan.Pednekar@us.ibm.com](mailto:emartens@us.ibm.com)

WW Product Manager, watsonx.data

**Evaluation Warning : The document was created with Spire.Presentation for Python**

Seller guidance  ![ref1]![ref1]

and legal  Slides in this presentation marked as **and**are for IBM and Business Partner use **Business PartnerInternal Use Only""IBM**  References in this presentation to IBM products, programs, or services do not imply that they will be available in all Product release dates and/or capabilities disclaimer and should not be shared with clients or anyone else outside of IBM or the Business Partners’ company.**AllRights Reserved.** referenced in this presentation may change at any time at IBM’s sole discretion based and are not intended to be a commitment 

countries in which IBM operates. 

© IBM Corporation 2023.  on market opportunities or other factors 

to future product or feature availability The information contained in this  in any way. Nothing contained in these publication is provided for informational  materials is intended to, nor shall have purposes only. While efforts were made  the effect of, stating or implying that any to verify the completeness and accuracy  activities undertaken by you will result 

of the information contained in this  in any specific sales, revenue growth, IBM and Business Partner  publication, it is provided AS IS without  or other results. 

Internal Use Only warranty of any kind, express or implied. 

In addition, this information is based on  All client examples described are presented IBM’s current product plans and strategy,  as illustrations of how those clients have which are subject to change by IBM without  used IBM products and the results they notice. IBM shall not be responsible for  may have achieved. Actual environmental any damages arising out of the use of, or  costs and performance characteristics otherwise related to, this publication or any  may vary by client.

other materials. Nothing contained in this 

publication is intended to, nor shall have 

the effect of, creating any warranties or 

representations from IBM or its suppliers 

or licensors, or altering the terms and 

conditions of the applicable license 

agreement governing the use 

of IBM software.

**Evaluation Warning : The document was created with Spire.Presentation for Python** 

Agenda **Introduction![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.004.png)**

Why should you care?

What is the opportunity?

Questions to understand customer need/ fit

**IBM Data Gate for watsonx solution** Solution components and architecture Capabilities

Demo

**Selling watsonx.data + IBM Data Gate for watsonx** Pricing and sizing

What customers need to buy

Who to get help from

**Evaluation Warning : The document was created with Spire.Presentation for Python**

**Why should you care?**

62% 70%

of organizations rated  rated application 

application modernization as a  modernization as a top 

top priority today priority in the next 2-3 years

1

Source: 

1\. [IDC Marketspace, Worldwide application modernization](https://www.ibm.com/downloads/cas/PRZOEAM4)

Challenges  ![ref1]![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.005.png)![ref1]

customers  **→systemsInvestmentsand codein  legacy/  →legacyDatasystemsmigrationarefromhard →  Business continuity risk** face with  **mainframe skills gap** • Don’t have  • Will I get the same availability or continuity mainframe  • Have been in production for decades compatibilities with newer modern formats that I have always enjoyed with modernization • These systems have accrued huge amounts  • The main reason to migrate is to save on  • mainframesI need 99.99XXX 

of data over the years license and maintenance  availability and not sure 

costs that any new platform 

- The original developers  can deliver that for my are either gone or retired • The applications that  applications that need to site on top talking to the  be available for my database are often the  customers

most complex and 

expensive to migrate

**Evaluation Warning : The document was created with Spire.Presentation for Python** 

Mainframe Data - an essential element  ![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.006.png)of any data Lakehouse strategy 

- Transactional data is essential to understand the  ![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.007.png)current state of the business 
- Transactional data is the most valuable data for  predicting business outcomes 
- For most enterprise organizations, transactional  data is kept on IBM Z 

11
**Evaluation Warning : The document was created with Spire.Presentation for Python![ref2]**

Questions on whether the client has a need or a fit![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.009.png)


**Evaluation Warning : The document was created with Spire.Presentation for Python![ref2]**

Questions

**How do you export data out of Db2 for z/OS today?**

**Do they have their own pipelines to move data out of  z/OS?**

**How do they maintain them?**

**Who makes changes to the pipelines?**

**What is your current compute infrastructure?  How much data?**

**What do you use today to implement your data warehouse strategy on mainframe data?**

**Have you looked at costs about modernizing or migrating from Db2 for z/OS to something else?![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.010.png)**

What to listen for

Listen for pain points related to the current way they move data outside of Db2 for z/OS… Ask if they manage this themselves or if they use an external partner.  If managed themselves who is responsible, how do they react to changes, e.g., upgrading to newer versions of Db2 for z/OS

Listen for problems with z/OS pipelines with Db2, IMS, and/or VSAM.  Try to drill down to how complicated these pipelines are from a technical 

point of view.  What happens when they do upgrades. And how much do they have to change these pipelines.  Is it only one person that manages these pipelines?  What happens if that person is away and something goes wrong?

Listen to problems of huge amounts of data being stored in Db2 for z/OS. IMS, and VSAM.  

Listen for how customer is currently moving data from the mainframe to other data sources.  Find out if they are IBM data sources or other data sources that we consider competitive… Find the pain points if data is being moved to competitive offerings. See if there are multiple copies of the data all over the place.

Migration costs are going to be huge.  The duration is going to be long.  Literally millions spent on parity at best? Have them spell out what they think it is going to cost.    

How can you position Watsonx.data

Watsonx.data is a very good way to augment your Db2 for z/OS environments.. Moving the data into iceberg format managed by watsonx.data means that the data still lives in the Db2 for z/OS but they have a better way modernize the data.

Let IBM provide a 24/7 enterprise supported solution so that even as tables are changing on the Z side, your application can still query the iceberg managed tables and get the same results as if the query were running on mainline Db2 for z/OS. 

Watsonx.data allows you to scale compute and storage separately so as your data storage needs grow you just add more storage nodes.. If your compute needs grow you just add compute nodes.  

Keep your transactional application data in the definitive version of the truth.. IBM Data Gate for watsonx is revolutionary, simple, efficient data synchronization.  Apply as much compute  for complex analysis as you need without impacting mainframe performance.  

Modernizing usage of the data is a good alternative to migration.  Db2 for z/OS excels at transaction processing.  Bring all the data to one place for multiple AI/Analytics use cases.Iceberg table format to share a single copy of data

21
**Evaluation Warning : The document was created with Spire.Presentation for Python![ref2]**

Today - complex integrations with IBM Z data leads to expensive solutions  

Cloud data warehouses / lake solutions become extremely  ![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.011.jpeg)expensive if treated like on-prem appliances  

Previously had fixed cost models and now charged based  on consumption 

Cloud warehouses are not optimized for “write” / “load”  operations which drive a huge amount of wasted  consumption 

~70% of all warehouse processing time is “write” oriented  meaning clients spend most of their cloud warehousing  spend on loading data vs. querying data for business  applications 

IBM Data Gate for watsonx

Beats competitive offerings with  ![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.012.png)

tangible added value for IBM Z data z/OS

- Provide an “easy” button for IBM Z  ![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.013.png)

  customers Transactional  ![ref3]![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.015.png)![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.016.png)![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.017.png)![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.018.png)![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.019.png)

queries ![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.020.png) watsonx.data ![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.021.png)![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.022.png)![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.023.png)

- The lowest possible latency and highest  ![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.024.png) ![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.025.png)![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.026.png)![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.027.png)possible throughput compared to other  Analytical  Queries 

  options Data Gate for watsonx 

- For Db2 for z/OS data, dramatically   **![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.028.png)![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.029.png)![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.030.png)![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.031.png)![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.032.png)![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.033.png)![ref3]**

  lowered overhead on the mainframe 

Analytical  

AI Queries

Act from a position of strength!  

Upsell Data Gate for watsonx to build on the value of watsonx.data

**watsonx.data**

Technical Value

Builds a lakehouse to 

optimize access to  –Store ONE copy of data![](Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.034.jpeg)

IBM Z workloads and  –Write data into an open format (Iceberg) integrates with  –Multiple analytics warehouses can read from Iceberg using the object storage of your choice

analytics & AI  –Built on open-source (Spark, Presto, Iceberg, database systems –Hive)Access enable distributed access to VSAM, IMS 

and Db2 data with a single solution

- Realtime access

  Financial Value

- Reduce Cloud Data Warehousing costs by +50%
- Eliminate legacy lake, warehouse and replication solutions costs
- Reduce MIP utilization attributed to data replication
91

[ref1]: Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.003.png
[ref2]: Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.008.png
[ref3]: Aspose.Words.6412a7be-4ac4-4ed5-8f00-cfc2c5f0dd80.014.png
