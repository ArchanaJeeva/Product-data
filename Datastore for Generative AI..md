**Evaluation Warning : The document was created with Spire.Presentation for Pythonwatsonx.data![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.001.jpeg)**

Datastore for GenAI![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.002.png)![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.003.png)

**Evaluation Warning : The document was created with Spire.Presentation for Python**

Agenda

**Introduction**

Problem spaces & challenges watsonx.data![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.004.png)

**The watsonx.data vector DB solution** Vector databases

RAG Use Case patterns

Milvus inside watsonx.data

**Pricing**

Pricing & sizing

When to use vectorDBs

**Use Cases watsonx.data**

Vector database examples

Financial Services – Generative Knowledge Use Case

**Learn More**

**Evaluation Warning : The document was created with Spire.Presentation for Python** 

Foundation Models  ...but how enterprises ![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.005.png)are bringing an  adopt and executewill inflection point in AI... definewhetherthey

unlock valueat scale ...meaningful GenAI 

starts with insightful data

**Evaluation Warning : The document was created with Spire.Presentation for Python**

**Generative AI expected to represent 30% of overall market by 2025.** IT and data leaders are faced with data challenges to scale AI models.

**Evaluation Warning : The document was created with Spire.Presentation for Python**

![ref1]

Multiple Data Modalities & Data Silos

Traditional databases are optimized for structured data in distributed locations.

AI today requires working with multiple modalities of data such as images, audio, documents which can be challenging.

![ref2]

Auditability

Businesses today are challenged with LLMs and AI models with unjustifiable data and hallucination. 

Businesses need support to ensure their data is reliable by using reference data.

48% believe decisions made by Generative AI are not explainable

![ref3]

Relevancy

LLMs and AI models today are not precise and relevant enough.

To get data to be precise you must augment your LLMs’ inputs with relevant business data.

![ref3]

Data Quality

Enterprise customers run the risk of inconsistent and low data quality on their AI models.

46% believe that GenAI will propagate established 

biases

Through integration with IBM Knowledge Catalog

**Evaluation Warning : The document was created with Spire.Presentation for Python**

Source: [https://www.idc.com/getdoc.jsp?containerId=US49018922)](https://www.idc.com/getdoc.jsp?containerId=US49018922)

**Evaluation Warning : The document was created with Spire.Presentation for Python** 

Empower your AI with  ![ref3]![ref1]![ref2]![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.009.png)![ref4]![ref4]![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.011.png)![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.012.png)![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.013.png)

Multiple Data  Auditability Relevancy

your trusted data.

Modalities & Data 

Silos watsonx.governance supports  watsonx.data’s Milvus 

as an end-to-end toolkit for AI  supports similarity search Leverage quality data  governance across the model  ensuring your data is 

for AI by unifying,  watsonx.aihandle multiple data  today can  lifecycle to accelerate  relevant and reliable.

responsible, transparent, and 

curating and preparing  modalities supporting a variety of open-source and  explainable AI workflows Augment your LLMs and AI data efficiently for AI  third-party AI tools Metadata and data lineage  models with the RAG pattern today using watsonx.ai or 

any supported AI tools. models and  Watsonx.data Milvus can  today will need to be stored with watsonx.data (to be augmented).

store any type of modality 

applications of your  that is in an embedding 

choice. format. brings together all your Watsonx.data

business data in one 

platform.

**Evaluation Warning : The document was created with Spire.Presentation for Python![ref5]**

Use Case Pain Points and Narrative

**Evaluation Warning : The document was created with Spire.Presentation for Python![ref5]**

Customer’s environment today

Enterprise customers are handling terabytes of data everyday needing to provide more insights and relevant context to their customers’ daily requests.

Customer Core Problem

The customer’s current LLMs aren’t accurate enough to share relevant insights and context to provide help to their customers. The customer is using a traditional warehouse and finds that training on their dataset is too complicated. Their data is scattered across multiple warehouses.![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.015.png)

Customer would like to easily capture their relevant data for them to train their LLMs and AI models. 

Talk Track

The solution here is to implement a RAG pattern using vector databases rather than traditional warehouses for data relevancy. ![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.016.png)

The customer needs to a single platform to connect their data across multiple sources that can be easily shared and accessed.

Value Proposition

Datastore for generative AI built into watsonx.data (Milvus) with provided IBM support and integrate with watsonx.ai and other support AI tools to train open-source models and LLMs in a hybrid-cloud environment. ![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.017.png)

Access across your existing data sources into a single shared metadata layer.

6


**Evaluation Warning : The document was created with Spire.Presentation for Python**Key Milvus Questions: Identifying the Problem

Questions What to Listen For What to do with results![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.018.png)

What type of data are you working with? • They are dealing with multiple data modalities including  • Watsonx.ai can handle all of these modality types

images, audio files, text embeddings, videos, documents,  • Advise customer to use watsonx.ai Foundation and others Models to support different modalities using open-

source models

- Customer may need to find third-party embedders:
  - Image: Imgbeddings, OpenL3
  - Text: Chroma
  - Video: Multimodal perceiver
  - Audio: OpenL3

What are the AI use cases you are looking to achieve? • They are looking to build AI models that involve RAG pattern: • Similarity search: 

What are the deployment patterns you are looking to get into? • Similarity search • Advise customer to use similarity capabilities 

- Recommendation system provided with Milvus
- Question & Answer system (natural language  • Recommendation system + Question & Answer system: processing) • Advise the customer to use watsonx.ai Prompt Lab to support Q&A and recommendation projects

How large is your dataset for your knowledge base? • Large datasets that traditional databases may struggle to  • If the customer’s data matches the left-hand side, the How many documents are you using? handle customer should be recommended to use watsonx.data What are the index types? • Look for documents ranging 100K+? Milvus

Do you need GPUs?  • FLAT, IVF\_FLAT, IVF\_PQ, HNSW, SCANN • If they need GPUs, the customer will be provided GPUs when 

- Determine if they need GPUs from us, or do they not need it? purchasing

What is your existing data infrastructure? • Look for the answer “no”, their current traditional data  • They will need watsonx.data Milvus and Spark to handle AI- Are you looking for a vector DB? sources are not keeping up with their AI-related workloads related workloads.

How are you working with embeddings today? • Look for open-source or third-party AI tools like Hugging  • Watsonx.ai also includes many open-source and third-party Are you working with embedding models today to generate  Face or Pytorch models in its Foundation Model feature

vector data for your AI workflows? • These tools can be used to convert their data modalities into  • The customer can continue using their AI tools in watsonx.ai

vector embeddings

Are you using a RAG use case pattern today? • They customer is already using RAG pattern today. Does their  • If the customer is not using watsonx.ai and would like to 

use case pattern follow one of the three categories (similarity  keep using their current AI platform, watsonx.data Milvus search, recommendation system or Q&A system)? can support the external AI platform

**Evaluation Warning : The document was created with Spire.Presentation for Python**

watsonx.data Milvus Vector DB![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.019.png)

What are Vector Databases?

A vector database is designed  What’s the difference between  ![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.020.png)![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.021.png)

to store, manage, and search  a Vector DB vs Regular DB? 

vector data, allowing for highly  ![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.022.png)![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.023.png)![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.024.png)

efficient and fast similarity  A vector database is a  searches.  

collection of data stored as  For example, in image or audio  mathematical representations.  

search, data with similar  ![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.025.png)

characteristics to a vector can  Vector databases make it  ![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.026.png)

be retrieved quickly. easier for machine learning  

models to remember previous  inputs, allowing machine  learning to be used to power  search, recommendations, and  text generation use-cases.

**\*Vector Databases on the Market**


**Evaluation Warning : The document was created with Spire.Presentation for Python**Vector Database Use Case Examples

You can use a vector database for Generative AI capabilities for use cases such as similarity search.

**Main Use Cases Description![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.027.png)![](Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.028.png)**

Image/Video similarity search • Prevention of copyright violations when sending outside the company

- Search for similar images of diagrams/photos in external documents
- Efficient collection of similar images for creating AI models

Personalized service and  • Recommends information and products based on the user's behavior, preferences, profile, proposal/recommendation systems and needs.

- Recommendations can be generated by finding vectors that most closely match the user's interests.

Question and answer system (natural  Vector search is essential to the use of Natural Language Processing and is used in multiple language processing) applications, including chatbots. It allows users to interact directly with the system by asking 

questions that are vectorized and matched to the closest match.

By representing data points as vectors, vector search provides a better semantic understanding of the query and more accurate results for each user.

[ref1]: Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.006.png
[ref2]: Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.007.png
[ref3]: Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.008.png
[ref4]: Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.010.png
[ref5]: Aspose.Words.1b8ce051-49d6-452b-b44e-d135ad94ab7b.014.png
