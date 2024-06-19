**Evaluation Warning : The document was created with Spire.Presentation for Python**

watsonx.ai ![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.001.png)![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.002.png)

Competitive insights 

Last update: May 2, 2024 

Seller guidance  ![ref1]![ref1]

disclaimer Slides in this presentation marked as **and**for IBM and Business Partner use and should not be shared with clients or anyone else outside of IBM or the Business **AllRightsBusinessReserved.PartnerInternal Use Only""IBM**are  References in this presentation to IBM products, programs, or services do not imply that they will be available in all countries in which IBM operates. Product release dates and/or capabilities referenced in this presentation may change at any time at IBM’s sole discretion based and are not intended to be a commitment to and legal  Partners’ company.

© IBM Corporation 2024.  on market opportunities or other factors future product or feature availability in any 

The information contained in this  way. Nothing contained in these materials is publication is provided for informational  intended to, nor shall have 

purposes only. While efforts were made  the effect of, stating or implying that any 

to verify the completeness and accuracy  activities undertaken by you will result 

of the information contained in this  in any specific sales, revenue growth, IBM and Business Partner  publication, it is provided AS IS without  or other results. 

Internal Use Only warranty of any kind, express or implied. 

In addition, this information is based on  All client examples described are presented IBM’s current product plans and strategy,  as illustrations of how those clients have which are subject to change by IBM without  used IBM products and the results they may notice. IBM shall not be responsible for any  have achieved. Actual environmental costs damages arising out of the use of, or  and performance characteristics may vary otherwise related to, this publication or any  by client.

other materials. Nothing contained in this 

publication is intended to, nor shall have  All statements in this report attributable to the effect of, creating any warranties or  Gartner represent IBM’s interpretation of representations from IBM or its suppliers or  data, research opinion or viewpoints licensors, or altering the terms and  published as part of a syndicated 

conditions of the applicable license  subscription service by Gartner, Inc., and agreement governing the use of IBM  have not been reviewed by Gartner. Each software. Gartner publication speaks as of its original 

publication date (and not as of the date of this presentation). The opinions

expressed in Gartner publications are not representations of fact and are subject to change without notice.”

**Evaluation Warning : The document was created with Spire.Presentation for Python** 

Contents • Overview of competitors![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.004.png)

- Competitive landscape 

  for generative AI

- Background on competitors
- Competitors’ key strengths      and weaknesses
- Competitor summary and watsonx.ai differentiators
- Objection handling
- Setting traps for competitors

**Evaluation Warning : The document was created with Spire.Presentation for Python**

Types of competitors **Hyperscalers Other generative AI** 

**vendors**

- Are experienced with  • Many startups or 

Generative AI is the next great innovation in  traditional AI  vendors who were Artificial Intelligence that builds on Foundation  modeling and  traditionally in other Models (with unlabeled data) where vendors  governance spaces (for example, support business use cases such as extraction,  Databricks) classification, text generation, summarizing, Q&A  • Supports open-

for Natural Language Processing (NLP) or even  source models and  • Many begin with coding language tasks. specialized models. variants of the GPT 

models and most There are two main categories of competitors: • Offer various degrees  provide some chatbot- of tuning  like capabilities.

- **The hyperscalers**: Amazon Web Services (AWS),  optimization and 

  Azure, Google Cloud Platform (GCP) some control • Most offer prompt 

engineering but not 

- Has resources to  much more
- **Other vendors** that are providing a generative AI  build proprietary 

  platform (AI21, Anthropic, Cohere, etc.)  models • Little to no  

governance on both 

- Offers API and often  data and models SDK for application 

IBM and Business Partner – Internal Use Only development

Competitor Overview

watsonx.ai ![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.005.png)

**Amazon**  Bedrock provides text and image models from multiple vendors (learn [more). Allows](https://aws.amazon.com/bedrock/) clients to easily test, fine-tune, and **Bedrock** deploy generative AI applications built with security and privacy in mind, SaaS only. Bedrock seamlessly integrates with 

Competitor existing AWS services such as Sagemaker Jumpstart. They also offer customizable “agents” for multistep tasks (learn [more)](https://aws.amazon.com/bedrock/agents/) and model evaluation and compare tool (in preview).![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.006.png)

Overview

|**Azure OpenAI** |Azure OpenAI Service, a part of Microsoft Azure's AI ecosystem, provides REST API access to OpenAI's advanced |
| - | - |
|**Service**|language models, including the GPT-4, GPT-4 Turbo with Vision, GPT-3.5-Turbo, and Embeddings. In preview (as of Dec |
||28) is Dall-E (Images from text) and Whisper (Speech to text)\. Azure also offers other models such as Davinci, Curie, |
||Babbage and Ada. Azure's offerings includes Azure Machine Learning for traditional AI and ML. Azure leverages Nvidia for |
||AI compute resources.|
|**Google** |Generative AI studio supports prompting and fine-tuning (incl. LoRa method of PEFT) of 130+ other first-party, open |
|**Generative AI** |source and third-party foundation models such as Gemini, PaLM2, Codey, Imagen, Chirp, BERT and FLAN. Google Vertex |
|**Studio, Vertex** |is a traditional AI and ML platform, now with links to the new Generative AI Studio for foundation models. Google has its |
|**AI**|own TensorFlow Processing Unit (TPU) for model building and also uses NVIDIA GPU. |
|**Nvidia**|NVIDIA is better known as a hardware vendor than a traditional AI vendor. However, as generative AI requires special |
||hardware, NVIDIA is in a unique position with its A100, H100 and L40S GPUs.    Its partnership with Azure is mutually |
||beneficial. NVIDIA has advanced imaging/video generative capabilities and offers NeMo, Picasso, and others.|
|**Cohere**|Cohere came from Google Brain experts. While they do not have traditional AI, Cohere is one of the stronger generative AI |
||startups with a close partnership with Google and targets developers. Cohere offers a fairly mature set of LLMs that |
||support embedding, text generating, and data-classifying use cases|
|**AI21**|AI21 offers LLM models with a focus on NLP use cases for enterprises and task-specific assistants (e.g. writing assistants). |
||Their LLM’s include Wordtune and the multilingual Jurassic series.  Their AI21 Studio provides private and secure API |
||access to their models for inference and fine-tuning.  It does not offer traditional AI capabilities. However, they do partner |
||with Amazon and others to provide broad access to their models.  |
|**Anthropic**|Anthropic is another startup with no traditional AI. Its LLM model Claude is ”Helpful, Honest, Harmless” – messaging to |
||address the general fear of generative AI risks. |

(Weaknesses 

not mentioned)

![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.007.png) **Databricks** Databricks is a traditional lakehouse shop (competes with watsonx.data and Cloudera which also is an IBM OEM.  . It has IBM and Business Partner – Internal Use Only traditional AI and is getting into generative AI via a June 23 $1.3B acquisition of MosaicML.  Their messaging focused on a data centric approach.  Governance is also prominent in their messaging.  Recently announced RAG.


**Evaluation Warning : The document was created with Spire.Presentation for Python**Competitive landscape Hyperscalers

|**Details**||![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.008.png) **IBM watsonx.ai**||**Amazon Bedrock![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.009.png)**||![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.010.png)||![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.011.png)|
| - | :- | - | :- | :- | :- | - | :- | - |
|**Deployment options**|•|IBM Cloud SaaS |•|AWS only|•|Azure SaaS Only |•|Google Only|
||•|Hybrid - customer managed software |||•|VPN access to client data |||
|||(on-prem)|||||||
|**Generative AI Tooling**|•|Watsonx.ai (Tuning Studio and |•|Bedrock|•|Azure AI Studio, Azure OpenAI Service,|•|Generative AI Studio, Document AI|
|||PromptLab)|•|SageMaker Jumpstart|•|Cognitive Search, Prompt Flow, OpenAI |||
|||||||Playground|||
||||||||||
|**Traditional AI Platform**|•|Watson Studio & Machine Learning |•|SageMaker|•|Azure Machine Learning|•|Google Vertex|
|||inside CPD|||||||
|**Generative AI models**|•|IBM models: Granite, Slate|•|Wide selection from AI21, Anthropic, Meta, Cohere, |•|Multiple OpenAI models such as GPT, DALL-E, |•|Google: BERT, BARD, FLAN, GEMINI, |
||•|Model library has growing selection of ||Stability, Huggingface||Codex||PaLM2, Imagen, Codey, Chirp|
|||LLM’s from partners such as Meta |•|Amazon models: Titan (text, image & embeddings) |•|Davinci, Curie, Babbage, Ada|•|Meta’s Llama 2, Anthropic Claude 2 |
|||and Huggingface|||•|Llama-2 and more||and more (130+ models)|
||||||||||
|**Hardware platform**|•|Nvidia A100, Vela, RHOS|•|Trainium cluster, Inferentia, Graviton|•|Nvidia cluster (A100, H100) GPUs,|•|TensorFlow Processing Unit|
||||•|Nvidia GPUs|•|Infiniband, NPU|•|GPU|
||||•|Supports Elastic Beanstalk|||||
Other competitors ![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.012.png)



|**Details**||||||![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.013.png)||||||![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.014.png)|
| - | :- | :- | :- | :- | :- | - | :- | :- | :- | :- | :- | - |
||||||||||||||
|**Deployment options**|•|Nvidia, AWS, |•|AWS, Amazon |•|AWS and |•|AWS and Google|•|AWS, Azure, |•|Github/manual|
|||Azure||Bedrock,   ||Google||||Snowflake|•|AWS, Azure, Google|
||•|On-premises||Google, Oracle|||||•|On-premises|||
||||•|On-premises|||||||||
|**Traditional AI Platform**|•|N/A|•|N/A|•|N/A|•|N/A|•|N/A|•|Databricks Machine Learning|
||||||||||||||
|**Generative AI models**|•|NeMo|•|Command|•|Wordtune|•|Claude|•|Mistral open and |•|Llama|
||•|Picasso|•|Generate|•|Jurassic||||commercial |•|MPT|
||•|BioNeMo|•|Embed||||||models|•|Dolly|
||||•|Classify|||||||||
|**Hardware platform**|•|Nvidia |•|Google|•|Google|•|Unclear|•|unclear|•|Unclear|
|||A100/H100|||||||||||

**Evaluation Warning : The document was created with Spire.Presentation for Python** 

AWS Amazon  ![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.015.jpeg)Bedrock 

**Amazon ![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.016.png)Bedrock** 

**Evaluation Warning : The document was created with Spire.Presentation for Python**

watsonx.ai

Competitor Background** information

Hyperscaler

Competitors Amazon Bedrock •• Bedrock GA’d in September, 2023Bedrock is seamlessly integrated with Sagemaker Jumpstart to provide a full suite 

of GenAI capabilities.

Background • Provides a wide range of models for both language and image generation use 

cases from partners such as AI21 Labs, Anthropic, and Stability.ai.  

- They also provide Amazon trained “Titan” series of models for language and 

[Recent News](https://ibm.box.com/s/uz0xdk2hha8v0beu0zg104ykkp1qngge) embeddings use cases and Titan Image Generator (In Preview) (link)![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.017.png)

**Amazon** • Supports wide range of tasks such as summarization, text generation, classification, **Bedrock** open-ended Q&A, information extraction, text and image search, image generation, 

embeddings

- Provides customizable agents, model evaluation and compare features (in preview as of Dec, 2023), and fine-tuning in a secure and private environment.
- Supports AWS developed cloud infrastructure (the Trainium series) which is optimized for GenAI inference processing.![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.018.png)![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.019.png)

IBM and Business Partner – Internal Use Only

**Evaluation Warning : The document was created with Spire.Presentation for Python**

![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.020.png)![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.021.png)

- Offers a combination of **IBM-trained, curated open-source, and third-party models** as well asBYOM
- Granite Series– **Trusted IBM-trained model covered by IBM product indemnification**
- Granite 13b – **Outperforms Llama 13b for RAG use case**
- IBM is **only provider that is transparent** about it’s model training methods and data sources
- **Target specific use cases for better performance** using** Prompt Tuning (PEFT)
- **Hybrid Cloud Deployment**workload portability and no vendor/hyperscaler lock-in
- **Bring Your Own Model (BYOM)**- Tune and host anywherewith watsonx.aifor supported architectures
- **Integrates seamlessly with watsonx.governance**for end-to- end lifecycle management, monitoring, and regulatory compliance

IBM Confidential

**Amazon Bedrock + Sagemaker![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.022.png)**

- Vendor lock-in – AWS models and tools are only available in AWS Cloud
- Titan and Anthropic are exclusively available in AWS (no client-managed options, ie on-prem)
- Anthropic is a startup – Indemnifying any large enterprise will be a challenge
- No foundation model transparency – AWS Bedrock models are nottransparent in terms of the data used to train theirfoundation models
- Disparate tooling – AWS hasa set of tools and APIs that users struggle to wire together to be productive
- No AWS native AI Governance solution – implementing governance after the fact is risky


**Evaluation Warning : The document was created with Spire.Presentation for Python**IBM watsonx.ai  = Broad support

Key comparisons  = Partial Support = No support

**AWS watsonx.ai![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.023.png)![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.024.png)![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.025.png)**

**Bedrock** Today

Today![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.026.png)

**Generative Models**



|Wide selection of models: ||||Wide selection of models: |
| - | :- | :- | :- | - |
|IBM Granite, Slate, Meta, select opensource models from ||||AI21, Anthropic, Meta, Cohere, Stability, Huggingface, |
|Hugging Face, **Granite – Trusted Model**||||Amazon|
|General purpose multilingual model support for|||||
|English, French, German, Spanish, Portuguese, Italian||||Multilingual Model support|
|Many more available through BYOM|||||
|Language specific models Japanese Arabic and Korean|**,**|||Language specific models|
|Multi-modal model support||Q2||Stable Diffusion XL|

**General Capabilities**

**Hybrid customer managed software (on-prem)**   No Hybrid, Only on AWS![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.027.png)![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.028.png)![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.029.png)![](Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.030.png)

Tuning

  Tuning

(prompt tuning available today, fine tuning in Q3)

[ref1]: Aspose.Words.a5c90046-0b60-47a8-a04c-91bb8214a2c7.003.png
