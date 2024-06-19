!
![ref2]



**Watsonx.ai Sizing Questionnaire**












*October 18, 2023*


<a name="_toc116705122"></a>*Collaboration and Deployment Services Installation on WAS and DB2*

!
![ref3]![ref2]

# <a name="_toc277666166"></a>Customer Information
Customer Name:

Date: 

IBM Consultant:

IBM Opportunity ID:

# Watsonx.ai components
Please select features you are planning to purchase/evaluate:

1. **Large Language Models:** Y/N
1. **Open source development tools:** Y/N
1. **Watson Machine Learning (WML) - Deployment:** Y/N
1. **AutoAI:** Y/N
1. **SPSS Modeler**:  Y/N
1. **Decision Optimization**: Y/N
1. **Data Refinery**: Y/N

*Note: you must provider answers or assumptions for questions in **bold**.* 

# Large Language Models and Generative AI
## **Models and use cases**
1. Which LLMs is the customer planning to use?

*Note: if the customer does not provide this information, we will recommend 6 VPCs (6 GPUs)*

1. Please provide a description of use cases

*Examples: summarization, Q&A with RAG, classification, sentiment analysis, named entity recognition, content generation, etc.*

## **Concurrent inference** 
1. What is the number of concurrent Prompt Lab users?

1. What is the number of concurrent requests *per second* from production applications?

1. What is the number of concurrent requests *per second* from test applications?

*Note: if the customer does not provide this information, we will use 60 requests per second from all 3 sources.* 

# Data Science
## **Open source**
1. How many users will be using open source tools in Watson Studio?

- **What is your estimate for *concurrent* number of users?**

- **How many vCPU (virtual processor cores) does each user need?** 

`    `*Recommended vCPUs per user is 2-4* 

1. Which languages/APIs are you planning to use (ex.: Python, R, PySpark, etc.)?

1. **Which IDEs are you planning to use?  (ex.: Jupyter, JupyterLab, RStudio)?**

1. What model types are you planning to build (SparkML, scikit-learn, Keras, TensorFlow, PMML, etc.)?

1. Are you planning to work with images (ex.: deep learning models)?

1. Are you planning to build text analytics models?

1. Dataset size for model building
- Approximate number of records for model building (largest data set):
- Approximate number of fields for model building: 

1. Data source types (databases, Hadoop, flat files, Excel, etc.): 

1. Are you planning to store data in WSL (flat files, images, etc) ?

- Approximate size of data :

1. Are you planning to use Remote Spark ? If yes, for what percentage of use cases?

1. Are you planning to run remote Python and R jobs (in a Hadoop cluster) ?  If yes, for what percentage of use cases?


## **AutoAI**
1. **How many concurrent AutoAI jobs are you planning to run?**

1. Dataset size for model building
- Approximate number of records for model building (largest data set):
- Approximate number of fields for model building: 

## **SPSS Modeler**
1. How many users will be using Modeler flows in Watson Studio?

- **What is your estimate for concurrent users of Modeler?**
- **Are Modeler users the same as open source tools users or is it a different group of data scientists?**

1. Dataset size for model building
- Approximate number of records for model building (largest data set):
- Approximate number of fields for model building: 

1. Data source types (databases, flat files, Excel, etc.) : 

1. Are you planning to use Text Analytics in Modeler ?

## **Decision Optimization for WSL (DO4DS)**
1. **How many users will be developing Optimization models (concurrently)?**

1. Dataset size for model building
- Approximate number of records for model building (largest data set):
- Approximate number of fields for model building: 

1. Data source types (databases, flat files, Excel, etc.) :

## **Data Refinery**
1. How many users will be using Data Refinery

- **What is your estimate for concurrent users of Refinery?**

- **Are Refinery users the same as open source tools users or is it a different group of data scientists?**

1. Dataset size that will be used in Data Refinery:

1. Data source types (databases, flat files, Excel, etc.) :

1. How many concurrent Data Refinery jobs are you planning to deploy?

## **Interactive or Scheduled Jobs in Watson Studio**
1. Do your data scientists need to run interactive or scheduled non-production batch jobs (for example, ETL or model building):

   1. If yes, approximately how many total number of jobs per day?

*Note: if the answer is not provide, the recommendation is to use 10% of concurrent user workload*




# Deployment
## **Open Source**
1. What type of assets do you need to deploy for scoring (models, notebooks, scripts, etc.)



1. Please describe the type of batch jobs (data transformation, scoring, etc.)
1. Model types (language, API – scikit-learn, etc, type - logistic regression, neural net, etc.)

1. **How many batch jobs do you need to run in a unit of time (concurrent workload)**

*Example:  need to run 10 jobs daily or 300 jobs in two weeks.*  

1. Dataset size for scoring
- Approximate number of records for scoring (largest data set):
- Approximate number of fields for scoring: 

*Note: if known, please specify number of records per job*

1. Data source types (databases, Hadoop, flat files, Excel, etc.): 

1. Are you planning to use Remote Spark ? If yes, for what percentage of batch jobs?

1. **Do you have models that need to be deployed for real time scoring?**


- **Approximate number of models:**
- Please describe frameworks (scikit-learn, TensorFlow, etc.)
- Real time scoring requests per second:

*Note: When calculating real time scoring requests, consider the number of models that need to be scored at the same time.*   

- Approximate number of input and output variables for real time scoring:

1. Is High Availability required for asset deployment in WSL?

1. **Number of AutoAI models you would like to deploy**

1. Batch:
1. Real time:

## **SPSS Modeler**
1. **How many batch jobs do you need to run in a unit of time (concurrent workload)?** 



1. Please describe the type of batch jobs (data transformation, scoring, etc.)
1. Model types (logistic regression, neural net, etc.)

*Example:  need to run 10 jobs daily or 300 jobs in two weeks.  Jobs can consist of one or more developed models.*   

1. Dataset size for scoring
- Approximate number of records for scoring (largest data set):
- Approximate number of fields for scoring: 

*Note: if known, please specify number of records per job*

1. Data source types (databases, Hadoop, flat files, Excel, etc.) : 

1. Do you have any models that need to be deployed for online scoring?

- Real time scoring requests per second:

*Note: When calculating real time scoring requests, consider the number of models that need to be scored at the same time.*   

- Approximate number of input and output variables for real time scoring:

## **Decision Optimization for WSL (DO4DS)**
The deployment of a DO model allows users and applications (internal and external to WSL Local) to execute the models. The number of users, complexity of the problem and expected processing time heavily influence the size of a Deployment environment. For example: “*the production planning model may run all night; processing time is irrelevant*”. Or “*this model will be used to schedule deliveries. It must run as fast as possible”.* With that in mind:

1. Estimate how many users and/or apps will be executing the Optimization models.
1. From question 1 above, estimate how many users/apps may run the models concurrently?
1. Will any mission-critical applications will utilize any of the deployed models?



# Infrastructure Requirements

1. Do you require isolation of *Development* and *Production* environments or will you deploy in a single watsonx.ai cluster? 

If yes, describe services and tasks that will be performed in each environment or select from recommended configurations.

*Note: Development environment in for data science requires a production license*

Recommended *Watson Studio Development Environment*:

- All tools (Notebooks, Modeler, AutoAIetc.)
- Smallest WML environment for testing

Recommended *Watson Studio Production Environment*:

- WML environment based on sizing, smallest configuration is 48 vCPUs
- Optional: smallest Watson Studio/Tools installation for making changes to scripts or notebooks 


1. Do you require non-production environment (used for testing, upgrades, etc.). 

1. If yes, how many?

1. What tasks will be performed in each environment?

*Example: fixpack testing, integration testing, performance testing*

# Other Comments


# Sizing Recommendations

This section will be completed by an IBM consultant and returned to the customer.  
\*


[ref1]: Aspose.Words.b9d5f55e-ede0-44cc-af13-4572e442c920.001.png "IBM_logoBlack10x4cmTransparent"
[ref2]: Aspose.Words.b9d5f55e-ede0-44cc-af13-4572e442c920.002.png
[ref3]: Aspose.Words.b9d5f55e-ede0-44cc-af13-4572e442c920.003.png
