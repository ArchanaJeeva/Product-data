watsonx ![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.001.jpeg)Foundation Models

Model Roadmap

Last update: June 5, 2024

Legal  References in this presentation to IBM ![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.002.png)![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.003.png)disclaimer T"OuIhsnBeilsM yap" n aridsen  sdfs oreh BnoutIuaBsltdMii nonn eaotsnmsdb a PBerak  usre shtd ina n ear eers s dIsn  w Pt aeit rrh tn nca elli r eU nstes   picmourodpnlyut rctihetsas,t  ipnthrogweyhr iawcmhil lsI bB, eorMa   opsvearielv ari acbteleess   id.n Po arnlodlotu  ct 

or anyone else outside of IBM or the  release dates and/or capabilities referenced Business Partners’ company. in this presentation may change at any time 

at IBM’s sole discretion based on market 

© IBM Corporation 2024.  opportunities or other factors and are not All Rights Reserved. intended to be a commitment to future product or feature availability in any way. The information contained in this  Nothing contained in these materials is publication is provided for informational  intended to, nor shall have the effect of, purposes only. While efforts were made  stating or implying that any activities to verify the completeness and accuracy  undertaken by you will result in any specific of the information contained in this  sales, revenue growth, or other results. publication, it is provided AS IS without 

warranty of any kind, express or implied.  All client examples described are presented In addition, this information is based on  as illustrations of how those clients have IBM’s current product plans and strategy,  used IBM products and the results, they which are subject to change by IBM without  may have achieved. Actual environmental notice. IBM shall not be responsible for  costs and performance characteristics 

any damages arising out of the use of, or  may vary by client.

otherwise related to, this publication or 

any other materials. Nothing contained in 

this publication is intended to, nor shall 

have the effect of, creating any warranties 

or representations from IBM or its suppliers 

or licensors, or altering the terms and conditions of the applicable license agreement governing the use of 

IBM software.

IBM and Business Partner Internal Use Only![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.004.png)
Foundation Models Roadmap *↷*

**watsonx watsonx![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.005.png)**

Client’s model needs → Model strategy→

Choices Multi-model

Enterprise-grade foundation models One model doesn’t fit all use cases. We offer IBM-

developed, open-source, 3rd party, and BYOM. Quality Bigger is not always better. Specialized 

models can outperform general-purpose Trusted platform to scale AI with confidence models with lower infrastructure requirements.

Multi-cloud

Control Deploy anywhere. We provide the flexibility to 

deploy models on the platform of choice. Reliable solution partner with deep AI expertise

**Available Models**

**IBM-developed models: 3rd party models:** • flan-ul2-20b ![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.006.png)

- granite-13b-v2 • granite-3b-code-instruct • llama-3-70b-instruct • flan-t5-xxl-11b

•• ggrraannititee--82b0-bja-mpaunlteilsine g ( uTaOlK only) ••• gggrrraaannnitititeee---823b04-bbc--occdooedd-eein--ininstssrtturrcuutcctt • llama-2-chat-13b • elyza-japanese-7b (TOK only)

(chat v2.1 and instruct) • llama-3-8b-instruct • flan-t5-xl-3b (Tuning Studio)

- llama-2-chat-70b • mt0-xxl-13b 
- granite-7b-lab • slate models • codellama-34b-instruct • llama2-13b-dpo-v7 (TOK only)
  - mixtral-8x7b • allam-1-13b-instruct (FRA only)
  - merlinite-7b • jais-13b-chat (FRA only)

![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.007.jpeg)

**Q1, 2024 Q2, 2024 2H, 2024![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.008.png)**

Performance

- granite-13b V2.1  • granite-13b-chat (2.1) • granite-8b
- Large, general-purpose models with OOB  • mixtral 8X7b1 • granite-7b-lab • granite 8X8b (English) performance on chat • BYOM Client-managed • llama 3-70b • mistral commercial 
- Specialized models that outperform general- • llama 3-8b models (starting with purpose models with lower GPU requirements • Embedding models Mistral Large and 
  - merlinite-7b (based on Mistral-7b) Mistral small)

Multi-lingual, regional

- granite-8b-japanese • granite-multilingual (1.1)
- Support for languages beyond  • granite-20b-multilingual • allam-1-13b-instruct (Arabic) English • elyza-japanese-7b • jais-13b-chat4 (Arabic)
  - mixtral 8X7b • llama2-13b-dpo-v7 (Korean)

Multi-modal • codellama-34b-instruct (16K  • granite-3b-code-instruct • granite 8X8b (Code)

- Support for code, text, image, video context) • granite-8b-code-instruct • Xb-code-base-long 
  - granite-20b-code-instruct (128K context)
  - granite-34b-code-instruct • Stability.ai

6
Supporting beyond English *↷*



|Supported Language|MZR availability|Models\*|
| - | - | - |
|Japanese|TOKYO|<p>IBM-developed model granite-8b-Japanese</p><p>**Granite**</p><p>3rd party model</p><p>- llama-3-70b</p><p>- elyza-japanese-7b</p>|
|French, German, Spanish, Portuguese |All regions|<p>IBM-developed model</p><p>granite-20b-multilingual **Granite ![ref1]![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.010.png)**</p><p>3rd party model </p><p>- llama-3-70b </p><p>- mixtral-8x7b</p>|
|Arabic|FRANKFORT|<p>3rd party model ![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.011.png)</p><p>- jais-13b ![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.012.png)</p><p>- allam-1-13b </p><p>- llama-3-70b </p>|
|Korean|TOKYO|<p>3rd party model ![ref1]![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.013.png)</p><p>- llama-3-70b-instruct </p><p>- llama2-13b-dpo-v7 </p>|
|Hebrew. European Languages (e.g., Dutch, Swedish)||<p>3rd party model ![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.014.png)</p><p>• Mistral commercial models (coming soon) </p>|
|Others (e.g., Turkish, Vietnamese)|Supported through BYOM|What BYOM lets customers do is to bring a model that is based on one of our supported architectures but tuned for their business needs. For example, using BYOM they can support additional languages like Turkish and Vietnamese.|

\*. The guidance is to lead with IBM models. Customers are encouraged 

to conduct testing on their specific language to evaluate performance. 6



Bring your own model *↷![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.015.png)*

Supported Architectures

**Model architecture  Supported quantization  Supports parallel ![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.016.png)***Available today* as client-managed software **type method tensors (multiGPU)**

bloom N/A Yes Coming Soon: BYOM SaaS in Q2 codegen N/A No

falcon N/A Yes

gpt\_bigcode gptq Yes FAQ  gpt\_neox N/A Yes

https:://ibm.seismic.com/Link/Content/DCB4MfMp3bGbjGmCj

cDdjGqHCJf3 gptj N/A No

llama gptq Yes Documentation for deploying custom foundation model mixtral gptq No https://www.ibm.com/docs/en/cloud-paks/cp- mistral N/A No data/4.8.x?topic=assets-deploying-custom-foundation-model

mt5 N/A No mpt N/A No t5 N/A Yes

7

Benchmarking, pricing, and differentiation data available at the [Model POV](https://ibm.seismic.com/app?ContentId=67b1842a-308c-48ba-bc1a-1e1f4ecdc4b7)

![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.017.png)

Model variety to cover enterprise use cases and compliance requirements

**Language Tasks**

Q&A ![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.018.png)Generate Extract Summarize Classify

**Coding Tasks**

CodeGen![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.019.png)

**Available in Tuning Studio**

Prompt Tune![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.020.png)

Model responds to a question in natural language Model generates content in natural language

Model extract entities, facts, and information from text

Model creates summaries of natural language Model classifies text (e.g., sentiment, group)

Model generates code from a natural language prompt Model can be prompt tuned

IBM Granite Model Series

*Decoder-only, generative models*

IBM Large Language Models![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.021.png)

granite-13b-instruct[^1] granite-13b-chat1 granite-20b-multilingual granite-8b-japanese granite-7b-lab

*13 billion params 13 billion params 20 billion params 8 billion params 7 billion params*

Extract Q&A Q&A Q&A Q&A Summarize Generate Generate Generate Generate Extract Extract Extract

Classify

Summarize Summarize Summarize Prompt Tune

Classify Classify Classify

This model will support English,  This model  This model German, Spanish, Portuguese,  supports Japanese supports and French InstructLab

IBM Code models  

granite-34b-code-instruct![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.022.png)

*34 billion params*

CodeGen

granite-20b-code-instruct

*20 billion params*

CodeGen

granite-8b-code-instruct

*8 billion params*

CodeGen

granite-3b-code-instruct

*3 billion params*

CodeGen

3rd Party Models

*Encoder/decoder & decoder-only Large Language Models available in Prompt lab*

*(Tuning NOT required for most tasks)*  1. 3rd Party LLMs have non-standard open-source 

terms with additional Acceptable Use Policies 

Open-Source Large Language Models 3rd Party Models1![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.023.png)![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.024.png)

flan-ul2-20b mt0-xxl-13b flan-t5-xxl-11b mixtral-instruct llama3-instruct llama2-chat elyza.japanese llama2-13b-dpo-v7 *20 billion params 13 billion params 11 billion params 8x7 billion params 70/8 billion  70/13 billion params 7 billion params 13 billion params* encoder/decoder encoder/decoder encoder/decoder decoder only *params* decoder only decoder only Korean model

decoder only

Q&A Q&A Q&A Q&A Q&A Q&A Translation Translation Generate Generate Generate Generate Generate Generate Q&A Q&A Extract Summarize Extract Extract Extract Extract Generate Generate

Summarize Classify Summarize Summarize Summarize Summarize Extract Extract

Classify Classify Classify Classify Classify Summarize Summarize CodeGen CodeGen Prompt Tune Classify Classify

jais-13b-chat allam-1-13b-instruct flan-t5-xl-3b *13 billion params* Codellama-34b- *13 billion params*

*3 billion params* Arabic model instruct  Arabic model encoder/decoder *34 billion params*

Translation Generate Summarize decoder only Translation Generate Summarize Prompt Tune Q&A Extract Classify CodeGen Q&A Extract Classify

IBM Slate Model Series

*Encoder-only, non-generative models*

IBM Foundation Models![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.025.png)

Slate (encoder-only) Natural Language Processing Models

Slate[^2]

*153 million params* multilingual distilled

Fine Tuning *Required* to support:

Extract

Classify

*See next page for IBM fine-tuned versions*

Fine-Tuned IBM Natural Language Processing Models

Encoder-only models, *already fine-tuned* by IBM for the specific tasks, based on the Slate ![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.026.png)model 

Slate Slate Slate Slate

*153 million params 153 million params 153 million params 153 million params* multilingual distilled multilingual distilled multilingual distilled multilingual distilled *Fine-tuned for  Fine-tuned for  Fine-tuned for  Fine-tuned for* 

*Entity Extraction Relationship Detection Sentiment Analysis Targeted Sentiment Analysis*

Extract Extract Classify Extract

Classify

Embedding Models For more Information:![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.027.jpeg)



|[https://dataplatform.cloud.ibm.com/docs/c](https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/fm-models-embed.html?context=wx&audience=wdp)||||
| - | :- | :- | :- |
|[ntent/wsj/analyze](https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/fm-models-embed.html?context=wx&audience=wdp)|[-data/fm](https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/fm-models-embed.html?context=wx&audience=wdp)|[-models](https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/fm-models-embed.html?context=wx&audience=wdp)|[-](https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/fm-models-embed.html?context=wx&audience=wdp)|
|[embed.html?context=wx&audience=wdp](https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/fm-models-embed.html?context=wx&audience=wdp)||||

![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.028.jpeg)

**watsonx.ai**

Foundation models  Tens of offered as a service + thousands of 

models1

Supported through BYOM (Bring **Q1, 2024 Q2, 2024 2H, 2024** Your Own Model) feature![](Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.029.png)

- **IBM-models Models in bold** 
- **IB**•••**Mggg-mrrraaaonnndiiittteeeel ---s 1823b0b-bj -aVmp2au.1nlt ei(lIsinne sgturaulctLab)** •• **ggrraanniittee--38bb--ccooddee** • **IBM**••••**-mGGGGorrrrdaaaaennnnlsiiiitttteeee----8MMxbbOO--EEcbo--a88dsXXee-88bbba--sbceoa-dsleeo-nbgase by select** 
  - **granite-7b-lab (InstructLab) are unique to** 
  - **2 embedding models (slate.125m.english.rtrvr  IBM SaaS and and slate.30m.english.rtrvr as of June 2024** 
  - **granite-20b-multilingual (InstructLab) are not hosted** 
- 3rd party models **(128K context length)**
  - mixtral 8X7b (quantized) • **granite-20b-code  competitors**
  - **elyza-japanese-7b**  • 3rd party models
    - **granite-34b-code** 
  - **codellama-34b-instruct** • stability.ai
    - Continuous delivery of the best 
- BYOM Client-managed • 3rd party models of 3rd party models as they 
  - llama 3-70b 

become available

- llama 3-8b 
- mixtral 8X7b (non-quantized)
- jais-13b (Arabic)1
- **allam-13b  (Arabic)**
- **merlinite-7b (InstructLab)**
- mistral commercial models SaaS *(coming)*
- **mncai/llama2-13b-dpo-v7 (Korean)**
- 3 embedding models (bge-large-en-v1.5, multilingual-e5-large, all-MiniLM-L12-v2)
- Mistral commercial models

15

Dates subject to change 1: Different Jais models are hosted by competitors

[^1]: . granite models support all 5 tasks (Q&A, Generate, Extract, Summarize, and Classify). .instruct is designed to follow short instructions and 

    returns concise response. chat is designed for human / agent conversations and question answering. We are finding that these models are multi - purpose. The chat variant for example might work very well for other use cases.
[^2]: . Slate models can be fine-tuned via notebooks and APIs. They support batch inference via Notebooks. No online inference. Batch inference supported in both CPU and GPU Notebook environments.
[ref1]: Aspose.Words.3eec8a43-1aca-4750-9432-cdd0e8300891.009.png
