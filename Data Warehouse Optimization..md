<a name="br1"></a> 

**Evaluation Warning : The document was created with Spire.Presentation for Python**

watsonx.data

Database Augmentation

Sales Play

Seller presentation

Anson Kokkat

[~~ansonk@ibm.com~~](mailto:ansonk@ibm.com)

WW Principal Product Manager, watsonx.data



<a name="br2"></a> 

**Evaluation Warning : The document was created with Spire.Presentation for Python**

Seller guidance

Slides in this presentation marked as "IBM

and Business Partner Internal Use Only"

are for IBM and Business Partner use

and should not be shared with clients

or anyone else outside of IBM or the

Business Partners’ company.

References in this presentation to IBM

products, programs, or services do not

imply that they will be available in all

countries in which IBM operates.

and legal

Product release dates and/or capabilities

referenced in this presentation may change

at any time at IBM’s sole discretion based

on market opportunities or other factors

and are not intended to be a commitment

to future product or feature availability

in any way. Nothing contained in these

materials is intended to, nor shall have

the effect of, stating or implying that any

activities undertaken by you will result

in any specific sales, revenue growth,

or other results.

disclaimer

© IBM Corporation 2023.

All Rights Reserved.

The information contained in this

publication is provided for informational

purposes only. While efforts were made

to verify the completeness and accuracy

of the information contained in this

publication, it is provided AS IS without

warranty of any kind, express or implied.

In addition, this information is based on

IBM’s current product plans and strategy,

which are subject to change by IBM without

notice. IBM shall not be responsible for

any damages arising out of the use of, or

otherwise related to, this publication or any

other materials. Nothing contained in this

publication is intended to, nor shall have

the effect of, creating any warranties or

representations from IBM or its suppliers

or licensors, or altering the terms and

conditions of the applicable license

agreement governing the use

IBM and Business Partner

Internal Use Only

All client examples described are presented

as illustrations of how those clients have

used IBM products and the results they

may have achieved. Actual environmental

costs and performance characteristics

may vary by client.

of IBM software.



<a name="br3"></a> 

**Evaluation Warning : The document was created with Spire.Presentation for Python**

Agenda

Introduction

What you should take away from this presentation

Questions to understand if the customer is a good fit

Database Augmentation Techniques

Penetrate existing accounts with watsonx.data

Attain new clients by prospecting competitor targets

Attack Databricks with Presto 2.0

Pricing / Competitive

Pricing and sizing

Competitive overview



<a name="br4"></a> 

**Evaluation Warning : The document was created with Spire.Presentation for Python**

What you should

take away from this

presentation

1

2

Position watsonx.data as an augmentation to

Db2 and Netezza not a replacement

Example: Modernize your on-premises Db2 or

Netezza appliance and optimize for AI

Augment and cost-optimize existing 3<sub>rd</sub> party

data warehouses either cloud or on-premises

Example: surround Snowflake with watsonx.data

Introducing watsonx.data new Presto 2.0 and

Optimizer+ features the fastest query engine on the

market

3

Example: watsonx.data with Presto 2.0 and

Optimizer+ has 60% better price performance than

Databricks



<a name="br5"></a> 

**Evaluat**

Q

**ion W**

u

**arni**

e

**ng :**

s

**The**

t

**do**

i

**c**

o

**ume**

n

**nt w**

s

**as cr**

t

**eat**

o

**ed wit**

u

**h Sp**

n

**ire.P**

d

**rese**

e

**nta**

r

**tio**

s

**n fo**

t

**r P**

a

**ytho**

n

**n**

d if a Customer has a need or fit

Questions

What to listen for

How can you position Watsonx.data

Emphasize Presto performance, scalability, and real-time analytics capabilities.

If their focus is on write orientated workloads talk about spark engine, and then talk

about the other features of Watsonx.data and see if they are interested and have them

look into it like bringing all your data together to one platform

What warehouse solution(s) they have in production today

What warehouse they have on cloud/on premise

Have they migrated any warehouse to a new platform

What would be the reason for the migration

How did you evolve your warehouse

overtime.

If they are using snowflake then talk about how Watsonx.data allows customers to leave

Snowflake in place for read oriented workload while executing write oriented workload

via a more optimized write-oriented engine.

Are they using a cloud warehouse engine like Snowflake.

Watsonx.data workload analyser tool can help customers gain visibility into where they

are spending money in write operations, with Watsonx.data they can choose the right

engine for the right workload at the right cost

Explain how customers can minimize risk by future proofing your data platform with

more flexibility/modularity with Watsonx.data

Vendor agnostic storage and open formats, standards to ensure interoperability with

future technology stack

Avoid incremental warehouse expansions that are driven by a storage scarcity

Listen for pain points such as

What is behind the cost?

What specific challenges are you facing

with your current warehouse?

What operations are costing the most in the warehouse cycle?

Any vendor lock in?

Not able support large workloads or any storage issues?

Assess the magnitude of their compute infrastructure and the volume of

data they handle to gain insights into critical factors such as scope and There are cheaper and better ways to store and process the data that customer can take

complexity

advantage of using watsonx.data

How big is your data warehouse

footprint? How big is your deployment?

Compute infrastructure cost are getting out of control

Customer feels they are paying a lot of money for the storage

Do they anticipate the need for a scalable solution that can handle

future growth in data volume

Talk about flexibly and scalability

Tailored customization of the data platform, allowing you to integrate and adjust

components based on precise business needs

If the customer mentions, Data marts – Emphasize how Watsonx.Data provides a unified

platform that integrates data storage, processing, and analytics capabilities in one place

transforming the customer's data management practices from traditional data marts and

warehouses to a modern, integrated Open Data Lakehouse approach

Data lakes - then you want to understand what type and then you start to ask about how

expensive is the write process. Position watsonx.data to modernize their data lake with

Multi-engine options to optimize costs and performance by pairing the right workload

with the right engine.

The diversity of data types the customer deals with, assess the

complexity of the customer’s data landscape

What are the primary sources of your

data that is feeding your analytical

warehouse

Understand type of data management tool

Are data landing in data marts first and then to warehouses or

Are they landed in data lake first and then moved to warehouse or

Do they land directly to the warehouse

**Note:** consider of what you found out about their data lake/ warehouse deployment and

ascertain whether delving into the next question would facilitate a deeper discussion on

data analytics and appropriately frame the context

IBM Software/© 2023 IBM Corporation

IBM CONFIDENTIAL



<a name="br6"></a> 

Questions to understand if a Customer has a need or fit

**Evaluation Warning : The document was created with Spire.Presentation for Python**

Questions

What to listen for

How can you position Watsonx.data

Reasons for Not Running Analytical Queries

Are you leveraging analytics on your large

Identify opportunities where introducing analytical queries could benefit the customer

Explain the benefits that analytics can help generate business insights with the data that

is available

Any challenges or pain points related to managing and accessing

data set?

data.

Any manual process

If **No** then

Are you leveraging analytics on your large

data set?

Are there workloads that’s are hot data that require highest

performance

Are there warm /cold data that doesn’t require high performance

Listen to what workloads can be offloaded? List of write-intensive

operations that are good candidates. What associated data needs to For write orientated workloads talk about spark engine

be offloaded as well?

Watsonx.data is a modern data lakehouse with Multi-engine options to optimize costs

and performance by pairing the right workload with the right engine.

If **Yes** then

In what ways is your data utilized for

analytics? generating reports, informing

decision-making processes or any specific

teams in your organisation use the data?

Emphasize Presto performance, scalability, and real-time analytics capabilities.

customer may mention data redundancy issues, when different group

Access data from data sources across the hybrid cloud in minutes

With Apache Iceberg table format share a single copy of data.

Emphasis on the removal of the need to duplicate data, move data.

require the same set of data, is multiple copies of data being made,

how is it handled?

Are there multiple copies of data out there

How are these multiple copies of data maintained

Has customers explored these alternative query engines for their

analytics workloads.

Is Prestro and trino giving the enterprise level support needed?

Is it good for long term business

For AWS Athena are you prepared to move all your data to the cloud find it useful

If they are using open-source presto, then talk about Enterprise support that IBM can

provide 24/7 worldwide

If they are not using Emphasise the benefits of presto, list out the benefits like Iceberg

table format to share a single copy of data, cost effectiveness, time travel, would they

Have you explored Presto, AWS Athena or

Trino?

Are the existing applications move to cloud , cost inquired not in

Are you on-prem or running on cloud? If on-

prem, what is the compute/storage infra +

how old?

control?

Ours is a multi-cloud solution that can be run on on-Prem or on cloud or a combination of

Are there limitations preventing the customers moving to cloud

Do they wish to have hybrid environment

both

If customers have old hardware they can consider running watsonx on fusion HCI

Our generative artificial intelligence (AI) tech stack includes all the components that

enable businesses to operationalize AI.

Place your data into watsonx.data for storage for all Retrieval Augmented Generation use

cases

Do you have any GenAI initiatives? What

strategies do you have in place for managing

the data required to support these

initiatives?

Customers might not know what option they have

What are they hearing for other companies who have deployed Gen

AI and their benefits

Datastore for generative AI built into watsonx.data (Milvus) with provided IBM support

and integrate with watsonx.ai and other support AI tools to train open-source models

and LLMs in a hybrid-cloud environment.

Access across your existing data sources into a single shared metadata layer.

IBM Software/© 2023 IBM Corporation

IBM CONFIDENTIAL



<a name="br7"></a> 

**Evaluation Warning : The document was created with Spire.Presentation for Python**

Penetrate Existing Accounts



<a name="br8"></a> 

**Evaluation Warning : The document was created with Spire.Presentation for Python**



<a name="br9"></a> 

**Evaluation Warning : The document was created with Spire.Presentation for Python**

Optimize data warehouse costs and modernize data lakes

Modernize analytics appliances:

IBM **watsonx.data**

– Co-sell & optimize workloads

between watsonx.data & Db2

Warehouse/Netezza for optimal

price/performance

**Data Warehouse**

Share

and promote data

Third party data warehouses:

**Generative AI** powered insights

IBM **Db2 Warehouse**

– Augment and cost-optimize

existing 3rd party data

warehouses, either cloud or on-

premises

**Presto** for analytics

**Spark** for ML and transformations

**Milvus** vector database for RAG

Share

and promote data

**Data Warehouse**

Governance

**Shared metadata**

Modernize existing Hadoop data

lakes:

IBM **Netezza**

– Modernize existing Hadoop-

based data lakes to a modern

analytics engine – watsonx.data

Modernize

data lakes

**Open** data and table formats

**Cloud object storage**

**Hadoop data lake**

**modernization**

**Open Data Lakehouse**



<a name="br10"></a> 

**Evaluation Warning : The document was created with Spire.Presentation for Python**

Extend warehouse data to Optimize workloads

your warehouse

Optimize costly warehouse workloads with

fit-for-purpose engines that scale

Gain new insights from your warehouse

data by combining [Db2 Warehouse and/or

Netezza] and watsonx.data platform data

through open formats engine.

automatically. Run resource-intensive

machine leaning (ML) model builds in your

watsonx.data lakehouse without impacting

business intelligence (BI) and dashboard

workloads in your warehouse.

**With**

**watsonx.data and**

**Db2 Warehouse**

**and/ or Netezza**

**you can:**

Share data through an

open format

Curate data

Use the watsonx.data lakehouse engine to

cleanse and transform data, reducing

complexity and time to prepare data for

model training. Easily bring lakehouse data

back to your warehouse as part of your

curated data set, ready for reporting,

analytics and AI

Eliminate data silos by sharing Db2 and/or

Netezza tables with data lakes and

lakehouse engines through open table and

data formats, such as Apache Iceberg,

Parquet, Avro and ORC, and CSV, JSON,

and more

