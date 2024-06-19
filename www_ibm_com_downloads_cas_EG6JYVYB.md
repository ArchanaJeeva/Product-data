The data store  ![](Aspose.Words.ce7f8d76-37e7-47ff-961f-fa313b6103b7.001.png)  for AI

![](Aspose.Words.ce7f8d76-37e7-47ff-961f-fa313b6103b7.002.jpeg)

Contents 01   05  

Introduction Cost optimization

opportunities

02  

The current state  06  

of data architecture Analytics and data

science enhancements

03  

The data  07  

lakehouse defined IBM watsonx.data

04   08  Components of  Next steps the architecture

![](Aspose.Words.ce7f8d76-37e7-47ff-961f-fa313b6103b7.003.png)

5 

Introduction

Previous chapter Next chapter 5


This ebook will examine the latest open data management solution for data and analytics leaders who want to significantly reduce cost, simplify data access and automate unified governance to scale AI. It s time for the data lakehouse.

Data is at the center of every business. It keeps applications running, powers predictive insights and enables better experiences for customers and employees. But the full benefit of data is elusive because of the way that data is stored and accessed for analytics and AI. 

You re not alone if you rely on monolithic repositories with multiple data warehouses and data lakes, on premises and on cloud; 82% of organizations are inhibited by data silos.1 And it s about to get worse: according to IDC, the amount of stored  data is expected to grow 250% by 2025.

The data lake was supposed to fix all these issues; just land your data in a centralized place and process it. But it s not so easy 

to update the lakes, properly catalog 

data or ensure good governance and 

the skillsets required for these tasks are specific, rare and expensive. As a result, data lakes have proven costly to build

and maintain. A data warehouse does offer high performance for processing terabytes of structured data. But warehouses can become expensive, too, especially for new and evolving workloads. Most organizations run analytics and AI workloads in 

2 ecosystems that are complex and cost 

inefficient. It s time for a change.

Previous chapter Next chapter 

` `250% ![ref1]![ref2]

The amount of stored data is expected to grow 250% by 2025.2 

Previous chapter Next chapter 9
12 

The current state of data architecture

Previous chapter Next chapter 12
13 

A combination of on-premises and cloud- native warehouses and bespoke data lakes is common for enterprise architecture today. You likely find that juggling cost, siloed data and data governance are constant challenges.

**Cloud orientation**

**Types of workloads![](Aspose.Words.ce7f8d76-37e7-47ff-961f-fa313b6103b7.006.png)**

**SaaS**  **SaaS** 

`  `Cloud warehouse  Cloud lake

**On premises**  **On premises**   Warehouse  Lake

High performance Low performance High cost Low cost

Small structure data Big unstructured data

Previous chapter Next chapter 13

The data lakehouse is an emerging paradigm ![ref1]![ref3]shift in how enterprises surface insights.3

Previous chapter Next chapter 6
4 

The data lakehouse defined

Previous chapter Next chapter 7
5 

Seek out a lakehouse solution that provides a modern data foundation to scale AI. ![](Aspose.Words.ce7f8d76-37e7-47ff-961f-fa313b6103b7.008.png)

The data lakehouse is an emerging architecture that offers the flexibility 

of a data lake with the performance 

and structure of a data warehouse. 

Most lakehouse solutions offer a high- performance query engine over low-cost storage in conjunction with a metadata governance layer. Intelligent metadata layers make it easier for users to categorize and classify unstructured data, such as video and voice, and semi-structured data, such as XML, JSON and emails.

The best data lakehouse will offer open- source technologies that reduce data duplication and simplify complex ETL pipelines. Be aware that some first- generation lakehouses have key constraints 

that limit their ability to address the challenges of cost and complexity. For example, a single query engine that s designed for business intelligence or machine learning (ML) workloads could well be ineffective when it s used for another workload type.

The IBM data and AI team believes that every workload is unique and should 

be optimized with the best-suited environment that keeps cost at a minimum and performance at a maximum. Choose a lakehouse that delivers an optimal level of performance for better decision-making, along with the flexibility that s necessary to unlock value from all types of data.

Previous chapter Next chapter 7

Figure 1. How to best scale   **watsonx.data ![](Aspose.Words.ce7f8d76-37e7-47ff-961f-fa313b6103b7.009.png)**

and accelerate the impact of AI

Multiple query engines

Metastore Object storage 

Structured data  Data lake

Unstructured data Data warehouse  Semi-structured data

Previous chapter Next chapter 8
6 

Components of  the architecture

Previous chapter Next chapter 9


Infrastructure 

This component is where your lakehouse will be deployed fully managed across any cloud or on-premises environment.

Storage

This layer is where the data is physically stored, which is stored as files and can be stored in open data formats, such as Apache Parquet and Avro. Open data formats are file specifications and protocols made available to the open- source community so that anyone can ingest and enhance them.

Open table formats 

Open table formats, such as Apache  ![](Aspose.Words.ce7f8d76-37e7-47ff-961f-fa313b6103b7.010.png)![](Aspose.Words.ce7f8d76-37e7-47ff-961f-fa313b6103b7.011.jpeg)Iceberg, help you provide structure, and  deliver the reliability and simplicity of SQL  with big data. These formats allow different  engines to access the same data, at the  same time which helps avoid vendor lock- in. Share data across multiple tools and data  repositories, such as your data warehouse;  

a single copy of data lets you reduce data  duplication and break down silos. 

Previous chapter Next chapter 9

04 Components of the architecture

Previous chapter Next chapter 10

Governance  

Metadata is also stored with open table formats; it serves to define the file formats for any tool that can read or write open data formats.

Technical metadata service

This component is required to understand what data is available in the storage layer. The query engine requires the metadata for the data and tables to provide full lineage and know where it s located, what it looks like and how to read it.

Data catalogs

This component helps users find the correct data for the job and delivers semantic information for policies and rules. Expect to store business metadata such as business terminologies and tags to enable search and data protection. 

Policy engine

This component enables users to define data protection policies and enables the engine to enforce those policies. To create a governance framework that’s scalable, a policy engine is often deployed with the technical metadata service and the data catalog. 

Query engine

This component is at the heart of the open data lakehouse. A query engine, which can be open source or proprietary, accesses data in open table format and is often known as the compute component. Query engines typically come in two types: an SQL-based query engine, such as the open- source Presto, or an open-source Apache Spark engine or its equivalent. 

In an open lakehouse architecture, the query engine is fully modular, which means that the engine can be dynamically scaled to meet workload demands and concurrency. Query engines can also attach to any catalog and storage.

Previous chapter Next chapter 10

` `50% ![ref1]![ref2]

Now it s possible to achieve faster,  trusted insights while you cut data  warehouse costs in half.4 

Previous chapter Next chapter 11
7 

Cost optimization opportunities

Previous chapter Next chapter 12


If your organization has existing on premises ![](Aspose.Words.ce7f8d76-37e7-47ff-961f-fa313b6103b7.012.png)![](Aspose.Words.ce7f8d76-37e7-47ff-961f-fa313b6103b7.013.jpeg)big data implementations, a lakehouse offers a less-expensive alternative for storing data in open formats on object storage. You ll lower the cost of analytics, decrease complexity and improve time to value. 

If you have an existing warehouse implementation, a lakehouse approach can represent a massively scalable, lower- cost alternative for your large analytics workloads that are less sensitive to service-

level agreements (SLAs). Warehouses are often expensive and proprietary 

but with a lakehouse, you can dramatically reduce storage and compute costs. You can optimize warehouse workloads using fit-for-purpose engines that are based

on your workload requirements. The open nature of a lakehouse frees you from proprietary warehouse technology, which means less vendor lock-in and a reduction in IT infrastructure overhead costs.

Previous chapter Next chapter 12

IBM watsonx.data is an open, hybrid, ![ref1]![ref3]and governed data store optimized for  

all data, analytics,  and AI workloads.

Previous chapter Next chapter 13
06 

Analytics and data science enhancements

Previous chapter Next chapter 14
06 

` `We are moving in the  Proprietary data formats and high storage direction where the  costs limit AI and ML model collaboration 

and deployments within a data warehouse data lakehouse becomes  environment; data lakes are challenged with 

a best practice. 3 low-performing data science workloads. The isolation of these technologies has led 

Adam Ronthal to downstream infrastructure challenges, Vice President  along with the security and governance Gartner implications that come with the duplication and movement of data for development of 

AI and ML models.

A data lakehouse is a great way to help colleagues who are hungry for the insights that lie waiting in your organization s data. If you re serious about extracting business value from the firehose of data that s coming at you, do consider the lakehouse strategy. 

Adam Ronthal, vice president and analyst at Gartner, says that  We are moving in 

the direction where the data lakehouse becomes a best practice. 2 The best approach will offer an open, collaborative and governed environment for the end-to- end management of data science workloads.

Let s examine IBMfi watsonx.data  the open, hybrid, and governed data store that s optimized for all data, analytics, and AI workloads.

Previous chapter Next chapter 14
07 

IBM watsonx.data

Previous chapter Next chapter 15
07 

Scale AI workloads, for all your data, anywhere. Watsonx.data is an open, hybrid, governed data store optimized for all data, analytics, and AI workloads, built on a data lakehouse architecture (see figure 1).

Access all of your data and maximize workload coverage across all your hybrid-cloud environments. Expect seamless deployment of a fully managed service across any cloud or on-premises environment. Access any data source, wherever it resides, through a single point of entry and combine it using open data formats. Integrate into your existing environment with open source and open standards, and interoperability with IBM and third-party services. 

Accelerate time to trusted insights. 

Start fast with built-in governance and automation; strengthen enterprise compliance and security with unified governance across your entire ecosystem. 

A clear UX and click-and-go console helps your teams ingest, access and transform data and run workloads. Watch how quickly they ll embrace a dashboard that makes it easier for them to save money and deliver fresh, trusted insights.

Reduce the cost of your data warehouse  by up to 50%4 through workload optimization across multiple query engines and storage tiers. Optimize costly warehouse workloads with fit-for-purpose engines that scale up and scale down automatically. Reduce costs by eliminating duplication of data when you use low-cost object storage; extract more value from the data in ineffective data lakes.

Previous chapter Next chapter 15
08 

Next steps ![](Aspose.Words.ce7f8d76-37e7-47ff-961f-fa313b6103b7.014.png)![](Aspose.Words.ce7f8d76-37e7-47ff-961f-fa313b6103b7.015.jpeg)

Take advantage of the IBM team s  data management and optimization  knowledge honed by decades of  handling the world s most demanding  data workloads. See how quickly you   can gain value from watsonx.data. 

[Start your free trial ](https://cloud.ibm.com/registration?target=/lakehouse&uucid=0b526df2f9c41d5f&utm_content=WXDWW)![](Aspose.Words.ce7f8d76-37e7-47ff-961f-fa313b6103b7.016.png)[Request a demo ](https://www.ibm.com/account/reg/us-en/signup?formid=DEMO-dataaiwatsonxdata)

Previous chapter 16



![](Aspose.Words.ce7f8d76-37e7-47ff-961f-fa313b6103b7.017.png)


1. Why Unstructured Data is the Future of   ' Copyright IBM Corporation 2023 Data Management, Venturebeat, July 2021.

IBM Corporation

2. Worldwide IDC Global DataSphere  New Orchard Road Forecast,2022-2026, IDC, May 2022. Armonk, NY 10504  
2. The rise of the data lakehouse: A new era   Produced in the United States of America of data value, CIO Magazine, 18 August 2022 May 2023 
2. When comparing published 2023 list prices  IBM, the IBM logo, and watsonx.data are trademarks normalized for VPC hours of IBM watsonx.data  or registered trademarks of International Business 

   to several major cloud data warehouse vendors.  Machines Corporation, in the United States and/or other Savings may vary depending on configurations,  countries. Other product and service names might be workloads and vendors. trademarks of IBM or other companies. A current list 

of IBM trademarks is available on ibm.com/trademark.

Statement of Good Security Practices: No IT system or product should be considered completely secure, and no single product, service or security measure can be completely effective in preventing improper use or access. IBM does not warrant that any systems, products or services are immune from, or will make your enterprise immune from, the malicious or illegal conduct of any party. 

The client is responsible for ensuring compliance with all applicable laws and regulations. IBM does not provide legal advice nor represent or warrant that its services or products will ensure that the client is compliant with any law or regulation.


It is the user s responsibility to evaluate and verify the operation of any other products or programs with IBM products and programs.

The performance data and client examples cited 

are presented for illustrative purposes only. Actual performance results may vary depending on specific configurations and operating conditions. THE INFORMATION IN THIS DOCUMENT IS PROVIDED 

` `AS IS  WITHOUT ANY WARRANTY, EXPRESS OR IMPLIED, INCLUDING WITHOUT ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND ANY WARRANTY OR CONDITION OF NON-INFRINGEMENT. IBM products are warranted according to the terms and conditions of the  

agreements under which they are provided.

17

[ref1]: Aspose.Words.ce7f8d76-37e7-47ff-961f-fa313b6103b7.004.png
[ref2]: Aspose.Words.ce7f8d76-37e7-47ff-961f-fa313b6103b7.005.png
[ref3]: Aspose.Words.ce7f8d76-37e7-47ff-961f-fa313b6103b7.007.png
