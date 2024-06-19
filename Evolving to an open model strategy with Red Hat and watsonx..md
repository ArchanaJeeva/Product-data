**Evaluation Warning : The document was created with Spire.Presentation for Python**

Evolving to an **open model ![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.001.jpeg)**strategy with Red Hat and watsonx.ai 

May 2024

**Agenda**

Part I  Model Strategy *and InstructLab*

Part II Red Hat and watsonx

Part III  watsonx fit *with models and InstructLab*

**Part I** 

Model Strategy

InstructLab: Disrupting Model customization 

Skills ![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.002.png)Making LLMs learn like we humans do:

Knowledge

Base Model with Knowledge and skills

© 2024 IBM Corporation

InstructLab uses a new alignment technique from IBM Research called LAB 

(Large-scale Alignment for chatBots)

1 2 3![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.003.png)![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.004.png)![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.005.png)

Taxonomy-driven  Large-scale  Iterative, 

data curation data generation large-scale 

alignment tuning

5

**Evaluation Warning : The document was created with Spire.Presentation for Python**Technology behind InstructLab (Large-scale Alignment 

for chatBots)![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.006.png)

![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.007.png) ![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.008.png) ![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.009.png) ![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.010.png)

6

Generate examples

High quality, hand-curated knowledge sources, plus a curated taxonomy of tasks with human- generated examples for each.

Teacher model(s) Critic model(s) Student model(s)

A teacher model generates  Critic models filter the  The student model is 

a “curriculum” of millions  questions for correctness and  trained with the 

of questions and answers  quality. Synthetic data is  curriculum using a novel for the taxonomies. scanned for prohibited material. training approach.

7
**Evaluation Warning : The document was created with Spire.Presentation for Python**

Our new LAB-aligned models achieve state-of-the-art chatbot performance.

8 ![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.011.png)7 

6 5 

4 MT-Bench 3 

2 

1 0 

Granite-13B Llama2-13B Mistral-7B

![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.012.png)Original Alignment ![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.013.png)LAB

8
**Evaluation Warning : The document was created with Spire.Presentation for Python**

Large-scale Alignment for chatBots for Code Models

Foundational

Knowledge Knowledge/Skill![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.014.png)

Private Public

Algorithms  Programming 

and Data  Language Syntax/PL LibrariesLibraries Stuctures Syntax

Programs/Compositional Skill


**Evaluation Warning : The document was created with Spire.Presentation for Python**

**Part II** Red Hat & watsonx.ai 

10

**Evaluation Warning : The document was created with Spire.Presentation for Python**watsonx.ai leverages the power of community that Red Hat 

OpenShift AI and RHEL AI offer



**watsonx.ai![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.015.png)**

Tuning Studio Foundation Models Data Science & 

Prompt Lab MLOps Toolkit

![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.016.png)

**RHEL AI** 

watsonx.ai **Multi-model flexibility Enterprise AI/ML lifecycle**

Access a variety of fit-for-purpose  Address LOB multi-user and organizational foundation models![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.017.png)![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.018.png) needs for scale and lifecycle governance

Red Hat  **Model serving & monitoring Resource optimization and management** OpenShift AI Deploy models anywhere with consistent  Create model pipelines for tuning and 

cloud-to-edge production deployment, and  alignment, validation and delivery; Share monitoring capabilities and optimize resources across teams

RHEL AI **Foundation model runtime engine Developer-friendly model toolkit**

Develop, deploy, and test open Granite  Bring rapid LLM experimentation to language/code models, supported &  developers via supported InstructLab CLI indemnified from Red Hat and IBM



Runs on any  ![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.019.png)![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.020.png)![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.021.png)![](Aspose.Words.e594a190-92ac-4474-b1aa-367a4a61f6d9.022.png)infrastructure 

Physical Virtual Private Public

