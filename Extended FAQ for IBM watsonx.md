Extended FAQ for IBM watsonx  

Table of Contents 

1. watsonx Platform Questions p. 2 
   1. General 
   1. Cloud Pak for Data – watsonx relationship 
   1. Data Fabric – watsonx relationship 
   1. IBM Watson – watsonx relationship 
1. watsonx.ai Specific Questions p. 7 
   1. General 
   1. GTM 
   1. Packaging/Sizing 
   1. Technical 
1. watsonx.data Specific Questions p. 19 
   1. General 
   1. GTM 
   1. Packaging/Sizing 
   1. Technical 
1. watsonx.governance Specific Questions p.26 
   1. General 
   1. GTM 
   1. Packaging/Sizing
1. Sales Specific Questions p.31 

watsonx Platform Questions 

Audience: Internal IBM leads  

Purpose: Alignment on watsonx messaging for broader content creation

- General 

What is watsonx?  

Watsonx is an AI and data platform with a set of AI assistants designed to help you scale and accelerate the impact of AI with trusted data across your business.

The core components include: a studio for new foundation models, generative AI and machine learning; a fit-for-purpose data store built on an open data lakehouse architecture; and a toolkit, to accelerate AI workflows that are built with responsibility, transparency and explainability.

The watsonx AI assistants empower individuals in your organization to do work without expert knowledge across a variety of business processes and applications, including automating customer service, generating code, and automating key workflows in departments such as HR. The three watsonx AI assistants are: watso[nx Assistant, ](https://ibm.seismic.com/Link/Content/DCWXcfbd733HC84FVFJRM8828jR8)[watsonx Orchestrate, ](https://ibm.seismic.com/Link/Content/DCbHf2RCFTPf3G9Cc2PBGggJWfGV)[watsonx Code Assistant. ](https://ibm.seismic.com/Link/Content/DC6VGC78Vc3jcG7MpCJ4BjG8XH2V)

How can watsonx can help my business?

Watsonx has been a game-changer for IBM's clients and partners, allowing them to scale and accelerate the impact of AI in their businesses with trusted data and governance. It's no surprise that companies in virtually every industry are turning to AI to enhance productivity and cut costs. With watsonx, businesses can rest assured that they have the support they need to succeed in the ever-changing world of AI. 

Many enterprises are achieving higher productivity by transforming their workflows into simpler, automated processes with the help of AI. To make this possible, IBM is collaborating with companies to apply AI in various areas, such as:

- enhancing internal audit and compliance processes, 
- optimizing cloud IT environments (resulting in a 75 percent reduction in infrastructure refresh costs), 
- automating hundreds of thousands of call center responses with over 90 percent 

  accuracy and increased client satisfaction, 

- enhancing cybersecurity to prevent real-time attacks from criminals, and 
- adding digital labor to finance, accounting, and HR teams to automate labor - intensive, data-entry tasks and save thousands of hours.

How will the 3 x’s work together from a technical POV?

Watsonx products are built on the common watsonx platform. This platform is built on OpenShift, establishes a common UI/UX, allows for common connectivity and product integration.  

What prompted IBM to rename/rebrand segments of its AI portfolio?

We’re at an exciting inflection point for AI. AI adoption among businesses is increasing, and we are seeing much more interest from businesses using AI to boost productivity and reduce costs.  

Watsonx gives new focus and brand identity to the IBM AI and data platform across our entire portfolio, featuring the latest generation of AI development, data management, AI and data governance capabilities. This enhances our ability to clearly communicate the platform's value and unique differentiation to our existing and future clients.

What clouds and locations will be covered for watsonx?

Watsonx is an AI and data platform that aligns with IBM’s Hybrid Cloud platform and will be supported on-premises and on any cloud. Initially, it will be available on the IBM Cloud, with broader deployment support to follow.

What are the availability dates for the components of watsonx?  

- Watsonx.ai will be available only on IBM Cloud initially in 3Q23 (July).
- Watsonx.data will be available on IBM Cloud and AWS in 3Q23 (July). 
- Watsonx.governance will be available only on IBM Cloud initially in 4Q23 (November). 

For more information on data center region availability, please review the IBM [SW Cloud Provider Roadmap in Seismic (p](https://ibm.seismic.com/Link/Content/DCMFgdgWT8mD6G9QW99XJ7qqJDVB)age 10). 

What is the roadmap to provision watsonx on AWS and Azure?

Our initial release is on IBM Cloud; we will then aggressively move to AWS and finally Azure. 

Please refer to the w[atsonx roadmap on Seismic for the](https://ibm.seismic.com/Link/Content/DCMmpHHmJchDq8qW3dM9TX8qjW9d) latest. 

Will there be any constraints using watsonx products in the local language?

Local language is not part of the GA. We expect local languages to be available in the future. 

Does watsonx run on OpenShift Container Platform (OCP)? 

Watsonx is fully aligned with our hybrid cloud software strategy and runs on OpenShift Container Platform. 

How will the watsonx subscription be structured? 

The watsonx subscription will allow you to provision and use watsonx.data, watsonx.ai and watsonx.governance. Technically, the subscription will allow you to install and provision any service in the cloud catalog. Shortly after GA, the subscription will be restricted to just the three core watsonx services.

What is the roadmap for other languages?

There are 5 languages targeted for multilingual models: Spanish, French, German, Japanese, Portuguese.  The timeline for delivery is TBD at the moment.

For more detail, refer to the [watsonx roadmap. ](https://ibm.seismic.com/Link/Content/DCMmpHHmJchDq8qW3dM9TX8qjW9d)

Does watsonx have Federal Certification?

FedRAMP for SaaS for watsonx.ai / .data / .gov is currently not in plan for 2023-2024. 

In the interim, on-prem / workaround for teams selling into USG / Federal are as follows:

- For watsonx.data – FIPS tolerant targeted to be available on-prem / containerized SW in 3Q2023. Fed clients will need to deploy .data in an environment that meets their needs. 
- For watsonx.ai – FISMA is targeted to be available on-prem / containerized for Q1 2024. 
- For watsonx.governance – is targeted to be available on-prem / containerized for H1 2024. 

What data management practices and technologies does IBM deploy to help clients develop enterprise-ready models and mitigate the risk of bias in model output?

IBM’s watsonx AI and data platform has an end-to-end process for building and testing foundation models and generative AI – starting with data collection and ending in control points for tracking the responsible deployments of models and applications – focused on governance, risk assessment, bias mitigation, and compliance. The watsonx platform enables clients to search for and remove duplication that improves the quality of output and use filtering and scoring technologies to decrease the chance that a system will include copyrighted material in the output.  IBM also puts thorough rigor into the development and testing of its foundation models, with contractual protections for IBM-developed generative AI products and models. As one of the first companies to develop enterprise AI, IBM’s approach to AI development is guided by core principles grounded in commitments to trust and transparency. Given the rapidly changing generative AI technology landscape, our end-to-end process will continuously evolve ![](Aspose.Words.10f87835-25ca-4b31-ba66-2c96582179f7.001.png)and improve.  

- Cloud Pak for Data - watsonx relationship 

How is watsonx different from Cloud Pak for Data (CP4D)? 

Watsonx is our AI & data platform, focused on AI builders, consuming data assets to build machine learning (ML) and generative AI applications. Cloud Pak for Data is a technology platform that uses a data fabric architecture, allowing data producers to understand and organize their data. Cloud Pak for Data will continue to support the data fabric architecture and enable data to be served up to watsonx, and power the next generation of ML and AI applications. You can’t build AI without training data.

Is watsonx available as a Cloud Pak for Data cartridge?

Generally, the watsonx subscription is a separate offering from Cloud Pak for Data, and is not an add-on to it. Although it shares some common core technologies at the OpenShift Container Platform level, it is available as a separate offering to serve the needs of our AI clients.  

IBM watsonx.data will be available at GA as SaaS, and also as a cartridge on Cloud Pak for Data.

When do we sell Cloud Pak for Data as opposed to watsonx?

Cloud Pak for Data is our integrated data fabric capability, serving key use cases such as data integration and data governance, allowing deployment of certain cartridges to extend its basic functionality. Watsonx is focused on AI builders. When clients have an AI-focused use case, watsonx should be the leading product.

What is the future of Cloud Pak for Data as a Service?

We will announce a new watsonx subscription that can be used with the AI services that are part of watsonx, i.e., Watson Studio, Watson Machine Learning, OpenScale, as well as new services and capabilities such as watsonx.data. For all other non-AI services, 

they will continue under Cloud Pak for Data as a Service subscription. Over time, we will review and enhance this subscription.

Will we have cartridges for watsonx like we do for Cloud Pak for Data?

None are planned now for watsonx as a whole. Watsonx.data is available as cartridge on Cloud Pak for Data. 

What is the co-existence strategy for Cloud Pak for Data and watsonx over the longer term? 

Cloud Pak for Data provides our data fabric foundation and helps clients collect and understand their data. Watsonx is complementary to Cloud Pak for Data by allowing clients to use the collected data for building AI applications. 

How are the watsonx platform and Cloud Pak for Data platform connected?

The watsonx platform is integrated with the Cloud Pak for Data platform so that current users of Cloud Pak for Data utilize existing OpenShift clusters for watsonx deployments. Although the platforms are distinct in UI/UX and product capability, the underlying infrastructure is utilized in a common way.

How will watsonx and Cloud Pak for Data software be sold together?

Software options will be sold concurrently. Perpetual, subscription, and monthly part numbers will be available for watsonx.data, watsonx.governance and watso[nx.ai. For ](http://watsonx.ai/)clients seeking services available in Cloud Pak for Data and Cartridges, we will maintain the existing parts for sale and renewal.

How will watsonx impact Embeddable AI?

The mission of Embeddable AI is to drive adoption of IBM’s AI technologies through ISVs such as SAP, Adobe, Salesforce, etc. Our strategy has been to position a focused subset of our software portfolio as Embeddable AI. Nothing changes on this front. In addition to existing products/libraries/APIs, a subset of wa[tsonx (e.g., fi](http://watsonx.ai/)ne tuning, inference) will be positioned to accelerate our foundation model adoption by ISVs. We will leverage standard commercial terms for watsonx at GA.

- Data Fabric - watsonx relationship 

What happened to data fabric?

Data fabric continues to be an essential underpinning of our clients’ data foundation. We continue to see significant adoption of our data fabric based on Cloud Pak for Data. Establishing a data fabric is a key step in our clients’ journeys to deploy effective and responsible AI. It allows them to catalog and understand all the enterprise data they need for model training tasks. 

What happened to the AI Governance use case from data fabric?

AI Governance is a critical component of watsonx. All features of AI Governance will come to watsonx over the ensuing months, including but not limited to the governance of foundation models (FMs). In short, you can think of watsonx.governance as "AI Governance ++". 

I am confused on how watsonx.governance is different from AI Governance? 

We are early to market with our AI Governance offering, when our competitors are still struggling to explain it. In fact, many vendors have no answer to this question, which gives IBM an opportunity to differentiate and get our clients’ AI into production. At launch in Q4, watsonx.governance will extend our existing AI Governance capabilities with support for foundation models and generative AI.

Are there any changes to the existing AI Governance narrative and messaging, impacting sales motion? 

Sales motions for AI Governance will continue normally. We encourage sellers to leverage the importance of AI explainability, transparency, fairness, and validation to generate discussions and position the AI Governance bundle. The AI Governance Bundle and the AI Governance Express Bundle (for AI sellers) should be positioned to clients interested in watsonx.governance components. Also, as usual, these components will be available as separate services both on-premises and on the cloud. An upgrade path will be made available to clients that purchase any AI Governance components today and wish to leverage the increased capabilities of watsonx.governance.

Does watsonx.governance include data governance?

Data governance and watsonx.governance are two separate offerings with different value differentiators. 

- IBM Watson - watsonx relationship 

How is watsonx different from IBM Watson and what does the rebrand mean for the future of Watson technologies?

Watsonx is an enterprise-ready AI toolset that uses trusted data and accelerates the building, deploying and governance of both machine learning AI models as well as the emerging category of foundation models for generative AI. Watson is the brand of IBM products that unlock new productivity levels by empowering individuals to make better decisions and deliver faster outcomes with AI and automation.  These capabilities, used by individuals and teams, are collectively called digital labor.

The AI capabilities of Watson products are built on watsonx, IBM’s AI and data platform that enables IBM clients and partners to scale and accelerate the business impact of AI with trusted data and governance. Introducing IBM’s AI and data platform as watsonx further demonstrates IBM’s commitment to continuing its leadership in AI for business that began with the introduction of Watson technology in 2011.

watsonx.ai Specific Questions

- General 

What is watsonx.ai? 

Watsonx.ai is the next-generation enterprise studio for AI builders. It combines traditional machine learning and new generative AI capabilities powered by foundation models into a powerful platform that enables you to build AI applications in a fraction of the time with a fraction of the data.  

Traditional AI tools, while powerful, can be expensive, time-consuming, and challenging to use. Data must be laboriously collected, curated, and labeled with task-specific annotations to train AI models. Up until now, building a model required specialized, hard-to-find skills — and each new task required repeating this process.

The introduction of foundation models provides a powerful and versatile foundation for a variety of AI applications. Clients can use foundation models to quickly perform tasks with limited annotated data and minimal effort; in some cases, users need only describe the task to coax the model into solving it. IBM’s new watsonx.ai studio offers a suite of foundation models aimed at delivering enterprise value. They’ve been incorporated into a range of IBM products that will be made available to IBM clients in the coming months.  

What services/products are represented by watsonx.ai? What are the product components underneath watsonx.ai?

Watson Studio, Watson Machine Learning, and the new generative AI.

What is the connection between watsonx.ai and Watson Studio?

Watson Studio provides the Machine Learning capabilities for watsonx.ai. Clients who want to leverage Machine Learning and AI lifecycle capabilities other than on IBM Cloud will still be able to purchase Watson Studio as they do today. However, clients who want to build AI with foundation models will need to buy or upgrade to an IBM Cloud SaaS subscription for watsonx. 

What documentation will be available for using watsonx.ai?

While the foundation model capabilities are in Tech Preview, a documentation tab will be available inside the application. When watsonx.ai is released, there will be standard documentation on IBM Cloud similar to what is available today for Watson Studio and other cloud products. 

How does IBM’s new partnership with Hugging Face play into watsonx.ai?

We have a shared commitment to delivering an open ecosystem approach that allows clients to define the best models and architecture for their unique business needs.  IBM and Hugging Face help clients select the best models, train, optimize, and run at scale: IBM provides security and support while clients get the flexibility provided by Hugging Face tools and open source. Together we build a better community through collaboration on open-source software for foundation models.  This partnership will allow our clients to innovate faster! 

Watsonx.ai will support the use of any open-source models hosted on Hugging Face. Also, IBM plans to make some of its own smaller models available on the Hugging Face platform for open-source use.  

How are the generative AI capabilities in watsonx.ai different from other generative chatbots (ChatGPT etc.)? 

Watsonx.ai is not a chatbot like ChatGPT. It is an enterprise studio for AI builders with the tools and runtimes needed to train, validate, tune and deploy traditional machine learning and new generation foundation models for prescriptive, predictive and generative AI tasks. It includes IBM foundation models that have been trained with one of the largest enterprise-relevant data sets, carefully vetted by IBM.

When will the tuning studio be available to use?

It will be available in 2H 2023. For more detail, refer to the wats[onx roadmap and ](https://ibm.seismic.com/Link/Content/DCMmpHHmJchDq8qW3dM9TX8qjW9d)[watsonx.ai model roadmap on ](https://ibm.seismic.com/Link/Content/DCVfj4mQD7jGT8qTC7gW3qJHWmHP)Seismic for the latest. 

When will Prompt Tuning be available?

Prompt tuning via the Prompt Lab interface is on the roadmap. It is scheduled to reach tech preview in early Q3.  Afterwards, it will be prioritized for production. ETA is to be determined. For more detail, please refer to the wa[tsonx roadmap and wa](https://ibm.seismic.com/Link/Content/DCMmpHHmJchDq8qW3dM9TX8qjW9d)tso[nx.ai model roadmap o](https://ibm.seismic.com/Link/Content/DCVfj4mQD7jGT8qTC7gW3qJHWmHP)n Seismic for the latest.

Is there a way for clients to test watsonx.ai ? 

We offer a free trial to clients who want to test our AI studio at a small scale for 30 days. Besides that, we connect clients in a programmatic approach with our Client Engineering, Sales and Consulting teams to evaluate best options for Generative AI use, reflected in [the AI Sales framework . ](https://ibm.seismic.com/Link/Content/DCQpX624hq2BWGFF78JjMQcGGj8P)

Where can I learn more about watsonx.ai? Start here in [Seismic. ](https://ibm.seismic.com/Link/Content/DCJH7MbqmMBmG8MPFjm2jWWfjgbP)

- GTM 

When will watsonx.ai be available to clients?

The current GA target is early Q3. Pricing details will be announced at that time.

For more detail, please refer to the wa[tsonx roadmap and wa](https://ibm.seismic.com/Link/Content/DCMmpHHmJchDq8qW3dM9TX8qjW9d)tso[nx.ai model roadmap on ](https://ibm.seismic.com/Link/Content/DCVfj4mQD7jGT8qTC7gW3qJHWmHP)Seismic for the latest. 

How will clients buy watsonx.ai? 

Initially, watsonx.ai will be available as a SaaS offering on IBM Cloud only. It will include end-to-end tools to leverage foundation models as well as existing Watson Studio capabilities. In 2024, the same set of features will be made available on-premises, multi-cloud deployments and on AWS. 

When can my clients start using watsonx.ai?

There is a Tech Preview Program administered by the Client Engineering team.  Learn more about the program [here. The](https://ibm.seismic.com/Link/Content/DC3gCVRC9CfJCGMRq3QhXJ448D88) Tech Preview currently features the foundation model library, prompt lab and APIs (note: tuning studio will be deployed to the Tech Preview server soon). Space in the program is limited. If you have a client with a use case, please fill out the application and the Client Engineering team will reach out.  The official GA of watsonx.ai is currently targeted for early Q3. I It will also include all the great Machine Learning capabilities of Watson Studio.

What are migration paths for existing clients?

After watsonx GA, existing clients can purchase a watsonx subscription which will allow them to access to the new foundation model capabilities. On-premises, watso[nx.ai  will ](http://watsonx.ai/)include the existing Watson Studio and Watson ML services, with extensions delivered over time to those services to better support wa[tsonx.ai's new ](http://watsonx.ai/)foundation model (FM) capabilities. Trade-up paths are being built to support Cloud Pak for Data 

to[ watsonx.ai sa](http://watsonx.ai/)les motions but will not be available in 2Q.

My clients want auto-provisioning of the generative AI capabilities if they have entitlement to Watson Studio. When will you make that available?

Watson Studio only provides ML features; generative AI and foundation models will not be made available to Watson Studio clients by default. They will have to upgrade to watsonx.ai. We are working on a client-friendly path to achieve this.

What is the Foundation Model Tech Preview Program? Learn more about the program, including how to apply here[.  ](https://ibm.seismic.com/Link/Content/DC3gCVRC9CfJCGMRq3QhXJ448D88)

How do the foundation models we host on [BAM comp](https://bam.res.ibm.com/)are against our competition (AWS, GOOGLE, MSFT)? 

IBM's play is to create smaller, enterprise-focused models which can sometimes outperform when operating “in-domain” or for a specific use case.  With our data provenance, IBM models will have fewer risks—and deployment costs.  They have also been optimized to work with our inference stack.  IBM Research will release performance metrics of our models in Q3. 

Strategically, it is not our intent to enter the arms race of "build a better model."  We envision a future where a client will select the best foundation model for a specific task and then bring their own data and start constructing the use case via prompt engineering or the tuning studio.

We are building tools to help them select the right foundation model as a starting point, even if it isn't a model from IBM Research. For clients who just want to get going quickly, we'll have multiple models "at the ready" on the platform.

For more detail, checkout the wa[tsonx.ai competitive insights asset i](https://ibm.seismic.com/Link/Content/DCM9h4qhBCmX2GHWWPVf6DWQj68j)n Seismic. 

Who are our competitors in this space?

Amazon Bedrock, Azure OpenAI Service, Google Generative AI, Cohere, Nvidia, AI21, Anthropic, and H2O.ai.  There are others such as Databricks and Palantir but these are more watsonx.data competitors who are now also dabbling in generative AI.

For more detail, checkout the wa[tsonx.ai competitive insights asset i](https://ibm.seismic.com/Link/Content/DCM9h4qhBCmX2GHWWPVf6DWQj68j)n Seismic. 

What are our competitors doing in this space? How do we differentiate?

Most of competitors are starting with LLM with Natural Language Processing (NLP) tasks. Nvidia is focused much more on image/video models.  Domain-specific areas like biology and others are beginning to emerge.  No one is tackling governance in a meaningful way; this aspect is still very new.  Most have a UI/API. For more detail, checkout the [watsonx.ai competitive insights asset](https://ibm.seismic.com/Link/Content/DCM9h4qhBCmX2GHWWPVf6DWQj68j) in Seismic. 

My client says they don’t want to participate in a workshop. Do we have a holistic, investigative method instead?  

Please see the Sales Play Spotlight page on Seis[mic that c](http://ibm.biz/GenAI-Spotlight)overs the AI Sales framework, including a programmatic approach on how to assess our clients’ AI readiness and how to engage with them via briefings, workshops, proof of value etc. here.  

- Packaging/Sizing 

What is the packaging/pricing structure for watsonx.ai? 

Watsonx.ai will be available as a SaaS at launch.

- For watsonx.ai (SaaS), customers will be charged a tier fee and consumption fees. 
- Tier Fees: The tier fee is a fixed per instance charge for access to all watsonx SaaS. Higher tiers grant access to additional capabilities. Tier fee does not cover consumption fees. For watsonx.ai SaaS, some or all watsonx.ai capabilities are included with the following tier fees:
- Trial: $0/month 
- Essentials: $0/month
- Standard: $1500/month
- Premium: TBD (not available at launch)
- Consumption Fees: 
- Foundation models are typically charged by 3 components: 
- Inference 
- Tuning\* 
- Hosting\* 

\*Capabilities only available with Standard and Premium Tiers

- Pricing for Foundation Models below (pricing in USD):

![](Aspose.Words.10f87835-25ca-4b31-ba66-2c96582179f7.002.png)

*IBM models will be offered in future watsonx.ai releases and charged at a premium versus OS models. Use-case specific models may be developed and monetized at specific rates.*

- Watson ML and Watson Studio: Pricing ($USD per Capacity Unit Hour) 
- Watson Machine Learning: Essentials ($0.52/CUH), Premium ($0.42/CUH) 
- Watson Studio: $1.02 / CUH 

Find more information on p[ackaging and pricing on Seismic.](https://ibm.seismic.com/Link/Content/DCJXVRXPCM3FB8cX3RWQQ4Pp6jdj)

What are the tier plans available for watsonx.ai and what do they include?

- watsonx.ai Saas is available with Trial, Essentials, Standard, and Premium watsonx Tiers. 
- Trial Tier: Standard Tier feature set. Credits are limited to 30 days and/or a $50 consumption cap whichever occurs first. Mapped to WML Lite plan at launch. Timebox not available at launch. 
  - ML functionality (20 CUH/month)  
  - Inferencing (25K Token limit/month)
  - Prompt Lab 
  - Opensource models 
- Essentials Tier:  
- ML functionality (20 CUH/month)  
- Inferencing (25K Token limit/month)
- Prompt Lab 
- Opensource models 
- Mapped to WML Standard plan at launch.  
- Standard Tier:  
- ML functionality (20 CUH/month)  
- Inferencing (25K Token limit/month)
- Prompt Lab 
- Opensource models 
- Mapped to WML Professional plan at launch. Includes $1,050 (USD) tier fee at launch.  
- Capabilities to be available in the future:  
- Prompt Tuning  
- Model hosting 
- BYOM 
- Synthetic Data 
- Premium Tier: In development. More details to be available later in 2H.

What are the system requirements for clients to host IBM Large Language Models (LLM)'s?  

For our SaaS offering in IBM Cloud, clients won't need to host models since they will be hosted by IBM.  For our on-premises offering, details have not yet been published but will be shortly.   

What IBM foundation models are included in watsonx.ai?

Recognizing that one size doesn’t fit all, we’re building a family of language and code foundation models of different sizes and architectures. Each model family has a geology-themed code name —Granite, Sandstone, Obsidian, and Slate — which brings together cutting-edge innovations from IBM Research and the open research community. Each model can be customized for a range of enterprise tasks.

Our Granite models are based on a decoder-only, GPT-like architecture for generative tasks. Sandstone models use an encoder-decoder architecture and are well suited for fine-tuning on specific tasks, interchangeable with T5 models. Obsidian models utilize a new modular architecture developed by IBM Research, providing high inference efficiency and levels of performance across a variety of tasks. All watsonx.ai models are trained on IBM’s curated, enterprise-focused data lake, on our custom-designed cloud - native AI supercomputer, V[ela.  ](https://research.ibm.com/blog/AI-supercomputer-Vela-GPU-cluster)

Efficiency and sustainability are core design principles for watsonx.ai. IBM Research has invented new technologies for efficient model training including our “LiG[O” algo](https://news.mit.edu/2023/new-technique-machine-learning-models-0322)rithm that recycles small models and “grows” them into larger ones. This method can save from 40% to 70% of the time, cost, and carbon output required to train a model. To improve inference speeds, we’re leveraging our deep expertise in quanti[zation, or ](https://research.ibm.com/publications/training-deep-neural-networks-with-8-bit-floating-point-numbers)shrinking models from 32-point floating point arithmetic to much smaller integer bit formats. Reducing AI model precision brings huge efficiency benefits without sacrificing accuracy. Our roadmap includes the ability to run these compressed models on our AI- optimized chip, the “IBM AIU.”  

Fm.language is a collection of enterprise-grade large language models (LLMs).  These models can drive both generative tasks (e.g., summarization) as well as traditional natural language processing (NLP) tasks (e.g., classification).  These models are built on IBM's trusted-data repository, and were trained with IBM's highly efficient LiGO technique, making them some of the most sustainably-trained foundation models available. 

For more detail, please refer to the wa[tsonx.ai model roadmap on Sei](https://ibm.seismic.com/Link/Content/DCVfj4mQD7jGT8qTC7gW3qJHWmHP)smic for the latest.

What traditional Machine Learning models are included in watsonx.ai?

The traditional, non-foundational ML models supported in Watson Studio today will also be supported in watsonx. 

These include: 

- [AutoAI ](https://www.ibm.com/cloud/watson-studio/autoai)and its many regression, classification, and forecasting models
- The hundreds of diverse open-source ML models in the scikit-learn library, along with the deep learning libraries of TensorFlow and PyTorch
- [Decision Optimization's CPLEX solver ](https://www.ibm.com/decision-optimization?p1=Search&p4=43700074457737984&p5=p&gclsrc=ds)
- SPSS Modeler's catalog of 50+ ML algorithms
- Watson NLP's suite of models 
- and many more... 

[A list of the supported ML frameworks for deployment can be found here.  ](https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/pm_service_supported_frameworks.html?context=wdp&audience=wdp)

It is widely known that foundation models are expensive to operate (e.g. $700K/day). How will IBM’s platform reduce the entry point for building and tuning models? 

The compute infrastructure is the largest cost associated with foundation models. The bigger the model, the higher the computation to process input and provide an output. That’s why the cost for a 100+B parameters is high. This is referred to as “usage” or “inference” cost and it is measured typically as price per 1K tokens. A token is approximately 750 words. You can think of it as asking a question that has 750 words. When you tune or fine-tune a model, you pay an upfront cost to lower the future inference cost. A tuned model will provide more accurate answers. Fine-tuning is very expensive, as it changes the underlying models. Tuning is a more cost-effective approach, since you don’t change the underlying model, and create an optimized prompt collection that allows the model to provide the output you need. 

Our focus for GA is on providing a more cost-effective approach through tuning, not fine - tuning. The issues with current tuning solutions are 1) complexity and 2) efficiency of the tuning algorithm. For example, the tuning stack for Vertex AI is two years old. We 

use the state-of-the-art Multi-task Prompt Tuning algorithm, paired with an easy-to-use guided tuning experience to make it easier for clients.

- Technical 

Can I add and use watsonx.ai to build with open-source models or others I have created? 

Yes, you can use the REST APIs and python sdk, which includes a LangChain integration, to build powerful AI applications.

What data domains and tasks are supported by the generative AI tools in watsonx.ai whether IBM provided the foundation models or I added them?

Watsonx.ai currently supports two domains: language and code. Foundation models in the language domain can support the following tasks: generation, summarization, classification, named entity recognition, and Q&A. The code domain is currently restricted to an open-source model (codegen-16b-mono), which can be used to write and explain code. New models will be added over time, including additional IBM-trained models. 

Will all foundation models currently in development by IBM Research be available in[ watsonx.ai? ](http://watsonx.ai/)  

IBM Research is actively working on developing foundation models across several enterprise domains. Some of these models currently in development will be made available in watsonx.ai.  

These include: 

- New additions to the fm.language model family.
- Ability to test and tune fm.code models (exclusively for IBM Watson Code Assistant Enterprise clients).

There are additional foundation models and capabilities in development that will be integrated into IBM products, and may be made available for select partners. 

These include: 

- Domain-specific fm.language models (such as bio, finance, cybersecurity)
- fm.geospatial models trained on remote sensing data that enable a number of downstream tasks such as flood detection and land use segmentation.
- fm.itevents models trained to diagnose and resolve IT issues.
- watsonx at the edge, a framework that enables deploying foundation models both on-premises and across a large number of edge devices. 

Although not available yet commercially, it is possible for clients to access these capabilities via a proof of concept (PoC) with IBM Research.

For more detail, refer to the [watsonx.ai model roadmap on Sei](https://ibm.seismic.com/Link/Content/DCVfj4mQD7jGT8qTC7gW3qJHWmHP)smic for the latest.

How and where is the client data used in watsonx.ai?

Client data is only used for prompt engineering, prompt tuning and fine tuning. IBM will not use client data for any other purpose. Clients retain full control of their data; they can delete it and any fine-tuned models they create at any time.

How does watsonx.ai manage bias and should I trust IBM’s foundation models?

IBM’s foundation models are developed, deployed, and validated using IBM’s industry - leading best practices in AI Governance. The data used to train IBM models was vetted for legal and safety concerns, and carefully curated by filtering out language reflecting hate/abuse/profanity, as well as removing duplicate data (note: duplicate data in the training set increases the risk of bias). You can learn more about the “[blue pile” process here. ](https://github.ibm.com/blue-pile/blue-pile).  

We are also working on techniques and capabilities to enhance the trustworthiness of foundation models throughout their lifecycle. We aim to minimize the bias risk in IBM’s foundation models by training our models on high quality datasets that are vetted for legal and safety concerns, filtered for language reflecting hate/abuse/profanity, and duplication. We are also actively researching debiasing techniques that can be applied throughout the foundation model lifecycle from data acquisition, model training and adaptation, to post-hoc auditing. 

Do watsonx.ai models hallucinate?

All generative models have some degree of hallucination (i.e., returning irrelevant or factually incorrect answers). Hallucinations typically occur when prompting a generative model on a topic that it was not trained for (or does not have sufficient data points in its training set).  

One of the best ways to reduce the risk of hallucination is to enable the model to retrieve relevant data related to a user’s query from a knowledge corpus before generating a final answer. This capability is called retrieval-augmented generation and is an area that we are actively pursuing. In the interim, watsonx.ai users are encouraged to read each model’s documentation and be aware of its intended uses, risks, and limitations. Users can also tune existing models to perform specific tasks which help to reduce hallucination risk. To learn more about hallucination, please see this [excellent IBM Tech video. ](https://www.youtube.com/watch?v=cfqtFvWOfg0) 

Where is my prompt data stored, and is it used for anything else?

Client data is stored in IBM Cloud with strict security and privacy requirements dictated by IBM’s CISO that includes fully auditable access records. Client data will never be used for model training.  

Can I tune a model in watsonx.ai and deploy it via the API? 

Yes, there is a 'Create Tune' API. Once trained, a tuned model becomes available for use through the GUI and API. 

If I tune a model and deploy it, can I monitor its usage?

Monitoring is limited to the current user’s session and the history of calls made through the Lab interface by that user. The ‘History’ API endpoint provides the ability to retrieve past generation requests and responses returned by the given models in the past 30 days. Currently, a user cannot monitor another user’s activity. 

Can users import third party foundation models, and will they be stored in the model catalog? 

Yes, there are two paths for importing 3rd party foundation models. One way is to import directly from storage with associated metadata. The other way will be to import models directly from an integrated vendor (e.g., HuggingFace). There will be an “import from vendor” feature that will walk the user through picking a model and accepting its license terms. In either case, after a model’s license terms are accepted, the model will be listed in the interface along with the other models. At the current time, users cannot upload their own models.

Are there accelerators for building new models?

We have a pipeline of data pre-processing and model training to accelerate model creation. We use this internally to build all our models; this same stack will be available over time to our commercial clients, beyond 2023. There are a few notable deployments of this training stack already with NASA for geospatial work, which will be highlighted at Think. 

Is there a play for Auto AI for foundation model building etc?

Classic machine learning lent itself well to “exploration-style” approaches to find optimal or near-optimal model architectures. Foundation models are different. 

While there is an opportunity to use tools, guides, and automation while building FMs, it will look different than the “exploration style” using Auto AI. 

For example, while building FMs, data cleaning and filtering are essential. The tools that automate and optimize this at scale are major accelerators. We’re in the early days of understanding which model architectures best fit different problems. There may be an opportunity for automation and model customization i.e. how we customize a base model for the task(s) needed. Right now, it depends on the user knowing what data to provide, how to configure the tuning, and which base model to select. The steps in the process could lend itself well to automated tuning.

Will clients be able to tune/optimize models?  

IBM provides approaches and tools to customize models from fine tuning (which is often most appropriate for smaller custom models) to prompt tuning to multi-task prompt tuning (a state-of-the-art approach to model customization). These capabilities will be in[ watsonx.ai (](http://watsonx.ai/)Tuning first, fine-tuning later) and are available directly through the underlying APIs. The key in model customization has been to provide the right user experience to guide a user to select which data is needed for customization, how much data, and how to configure the tuning job.

Where can I find documentation and custom training models?

Since we aren't offering the ability to train GenAI LLMs at GA in July, specific info for training models will be released later as part of the tuning studio in watsonx.ai. For the Watson Studio NLP LLMs: documentation can be found here in Ov[erview  and ](https://medium.com/@alex.lang/watson-natural-language-processing-comes-to-ibm-watson-studio-notebooks-a81802dee9c8)in [the documentation here.](https://ibmdocs-test.dcs.ibm.com/docs/en)

Are prompts preloaded with the recommended model type? Can users compare model results side-by-side or receive automated recommendations after testing different models? 

The sample prompts will be displayed with the default (and most optimal) model and parameters.  However, these can be changed prior to generating responses to experiment with the outcomes.  There is a feature currently in the backlog to add a side - by-side output comparison, but it's not likely that this feature will make it into production by the end of 2023.

watsonx.data Specific Questions

- General 

What is watsonx.data? 

To scale analytics and AI workloads, organizations are adopting data lakehouses, which combine the performance of data warehouses and the flexibility of data lakes on low - cost object storage. Watsonx.data is the industry’s only open data store that enables you 

to leverage multiple query engines to run governed workloads wherever they reside, resulting in maximized resource utilization and reduced costs.

Built on an open data lakehouse architecture, watsonx.data allows you to access all your data through a single point of entry across all clouds and on-premises environments. Clients can get started in minutes with built-in governance, security, and automation.  Watsonx.data leverages open data formats and low-cost object storage for flexibility and simplicity.  Clients can reduce their data warehouse costs by up to 50% through workload optimization. 

Watsonx.data allows clients to take advantage of fit-for-purpose query engines like Presto and Spark that optimize workloads for all data types, ensuring fast and efficient processing for high-performance querying, BI, reporting, and machine learning at scale. With shared metadata and access management, watsonx.data is built to manage the ever-expanding data volumes and most sensitive enterprise workloads on-premises, or in the cloud. Supported by built-in integrations with their databases, tools, and modern data stack, clients can leverage IBM’s extensive partner ecosystem, and deep i[ndustry and technical expertise through IBM Consulting. ](https://www.idc.com/getdoc.jsp?containerId=US49018922)

How is watsonx.data unique, first of a kind, or differentiating?

- Multi-engine architecture – Optimize warehouse workloads using fit-for-purpose query engines including Presto and Spark that support all data types and workload needs. Modernize data lakes with warehouse-like capabilities.  
- Governed data across the enterprise – Protect data, manage compliance, and maintain trust with built in-governance, access controls, and enterprise security. Integrate with IBM watsonx.governance to enable responsible, transparent and explainable data and AI workflows across the enterprise.
- Access to all data, anywhere - Deploy anywhere with full support for hybrid-cloud and multi cloud environments

What is the role of foundation models within watsonx.data?

Foundation models are used to automate data search, discovery and linking in watsonx.data. [Click here for more information.  ](https://secure.video.ibm.com/channel/23354459/video/132862540)

What is the connection between watsonx.data and IBM’s recent acquisition of Ahana? IBM has selected Presto as one of the pillars of its Data Lakehouse infrastructure. Ahana is a leading contributor to the Presto engine. IB[M acquired Ahana to hel](https://www.infoworld.com/article/3693453/ibm-acquires-saas-based-prestodb-provider-ahana.html)p make it the best engine for data lakehouses.

How does the launch of the data lakehouse fit with IBM's data fabric strategy?

IBM’s data and AI market leadership, mo[st recently demonstrated by its i](https://www.ibm.com/blog/ibm-named-a-leader-in-the-forrester-wave-data-management-for-analytics-q1-2023/)nclusion in The [Forrester Wave: Data Management for Analytics, exte](https://www.ibm.com/account/reg/us-en/signup?formid=urx-52056)nds to watsonx.data by integrating with existing IBM solutions like StepZen, Databand.ai, IBM Watson Knowledge Catalog, IBM zSystems, IBM Watson Studio, and IBM Cognos Analytics with Watson. This enables users to utilize various industry-leading data catalog, lineage, governance, and observability solutions across their entire data ecosystem.

Watsonx.data seems nothing more than a rebranding of IBM Lakehouse. What is the AI value proposition of .data? Will it have any real integration with watsonx.ai?

IBM Lakehouse was an initial name for our new modern AI repository that supports the data lakehouse pattern. This will now be referred to as watsonx.data as part of the watsonx platform. The three services of the platform (.data,.ai,.governance) are all integrated to provide end-to-end capabilities to support AI builders.

Where can I learn more about watsonx.data? Please start here in S[eismic. ](https://ibm.seismic.com/Link/Content/DCbbPfP64CX3RG4CJPH7bH8XjGBP)

What if I have more questions on watsonx.data? Please check out the [watsonx.data specific FAQ doc. ](https://ibm.seismic.com/Link/Content/DC24pQJX7c4M7GCRFM8FqQmTHTQG)

- GTM 

Who is the intended user for this product?

Data Engineers, Data/Business Intelligence Analysts, Data Scientists, Database/Data warehouse admins (DBAs), Enterprise Architects

When will watsonx.data be available to clients?

The product was announced in beta at Think 2023, but will available via a SaaS offering in 3Q’23.  

Refer to the [watsonx roadmap on Seismic for th](https://ibm.seismic.com/Link/Content/DCMmpHHmJchDq8qW3dM9TX8qjW9d)e latest. 

How and where do clients buy watsonx.data?

Watsonx.data, IBM Db2 Warehouse, and Netezza Performance Server are offered as fully managed SaaS services on IBM Cloud and AWS. They are also available as self - managed containerized software on Red Hat OpenShift.

Do you have any clients who are currently testing or using the beta? 

Yes, we have 11 clients actively using the beta today with another 16 onboarding. The clients range from local government to Fortune 500 companies.  Please reach out to the watsonx.data team directly for more information or leverage this beta [enablement deck. ](https://ibm.seismic.com/app#/doccenter/861ea1fd-99e0-44d7-9135-85412e5c28d1/doc/%252Fdd3359e5f7-a856-a91b-7688-41024b2ac637%252FdfNTY4NmVhOWItY2RkNS04ZWY3LTZkNzItZTQwZjczMWUyMjk1%252CPT0%253D%252CRGF0YSBhbmQgQUk%253D%252FdfOthers%252FdfOTRiYmU4NTQtNWY4NC03Y2QyLWZjYWUtOGIxYmFmZjkyZThk%252CPT0%253D%252CU2VsbGVyIGVuYWJsZW1lbnQ%253D%252Flf9a67eed0-3270-4509-a59e-6683b6b3f4af//?mode=view&parentPath=sessionStorage)

What will a client use watsonx.data for? Can you provide 2-3 use cases or examples? Today most large enterprises have a mix of data repositories and data stores in hybrid environments to manage their data and workloads. The overall cost across all these repositories remains high and it has become difficult for enterprises to effectively leverage the data across multiple environments and use their data for analytics and AI. Organizations can use watsonx.data to optimize costly data warehouse workloads with low-cost object storage and fit-for-purpose query engines and extract greater value from data in ineffective lakes by modernizing and bringing warehouse-like capabilities.  

1. Access to all data across hybrid-cloud environments  

Share a single copy of data with tools that can read open data formats to minimize data duplication. Connect to and access data remotely across hybrid-cloud with the ability to cache remote sources. Deploy seamlessly on-premises and within a managed service on any cloud environment. 

2. Get started in minutes with built-in governance, security, and automation 

Connect to data in minutes with full-service storage, metastore and engine -- all integrated and preconfigured. Address enterprise compliance and security management using built-in unified governance across your client’s data ecosystem.

Discover, augment, refine, visualize IBM watsonx.data data and metadata in a conversational UI experience.

3. Reduce the cost of data warehouse storage by up to 50%\* through workload optimization across multiple query engines and storage tiers:

Clients can optimize workloads from their data warehouses by taking advantage of fit for purpose engines that can scale up/down automatically. Presto and Spark, both of which are supported by an Intel processing foundation, offer quick and reliable data processing for high performance SQL querying, reporting, business intelligence, and machine learning at scale.  Further, this helps reduce costs by eliminating duplication of data utilizing object storage, and helps extract better value from data in ineffective data lakes by modernizing and introducing warehouse-like capabilities.  

\*When comparing published 2023 list prices normalized for VPC hours of IBM Lakehouse to several major cloud data warehouse vendors.  Savings may vary depending on configurations, workloads and vendors. (Footnote must remain with claim according to the Legal department)

Who are the key competitors we are targeting with this solution and how is IBM's solution better for clients?

Watsonx.data is the industry’s only open data lakehouse that can run across multiple clouds and on-premises. Unlike competitors, it supports fit-for-purpose query engines to optimize workloads for both cost and performance at scale. 

Key competitors include: 

- Snowflake  
- Databricks 
- Dremio 

Are you targeting specific industries with this solution? If so, which ones and why? We’re not targeting specific industries at the moment. 

- Packaging/Sizing 

Are other partners or IBM products involved in the watsonx.data product? If so, how and what role do they play? 

Watsonx.data will incorporate the latest performance enhancements to the Presto open - source query execution engine via Velox, which is being developed in collaboration with Intel and Meta. Watsonx.data will also incorporate IBM’s Storage Fusion technology to enhance data caching across remote sources and semantic automation capabilities based on IBM Research’s technology on foundation models to automate data discovery, exploration, and enrichment through a conversational user experience. It provides full flexibility with open source and open standards, and interoperability with IBM and 3rd party services. There are optional integrations with the rest of the IBM portfolio including Watson Knowledge Catalog, Cognos, DataStage, StepZen, and more. 

What is the packaging/ pricing structure for watsonx.data?

- watsonx.data Software (Not SaaS)
- Price Metric: VPCs (16 VPCs/node) @ $7500/VPC 
- Minimum of 10 nodes recommended.
- Production versions available in Perpetual, Subscription and Monthly Licenses. Options for Non-production, reserved, and various support tiers also available. 

  **License Type   Price (USD) / VPC**  Perpetual   $7,500  ![](Aspose.Words.10f87835-25ca-4b31-ba66-2c96582179f7.003.png)Subscription   $250 / month  ![](Aspose.Words.10f87835-25ca-4b31-ba66-2c96582179f7.004.png)Monthly   $312.50 /month  

- On-prem Parts are listed [here. ](https://ibm.ent.box.com/file/1250792328939?s=hyd5de29lliy4numkiuyhic86656xyeo)
- No tiers or tier fees are planned for watsonx.data Software as this time.
- watsonx.data SaaS 
- For watsonx.data SaaS, customers will be charged a tier fee and consumption fees.  
- The tier fee is a fixed per instance charge for access to all of watsonx SaaS. Higher tiers grant access to additional capabilities. Tier fee does not cover usage fees. For watsonx.data SaaS, watsonx.data capabilities are included with the following tier fees: 
  - Trial $0/month 
  - Standard $1500/month 
  - Premium: TBD (not available at launch)
- Watsonx.data’s consumption fees are based on three price metrics. 
- Quantity of nodes deployed
- Duration of nodes deployed
- Support services deployed (e.g. Hive, Ranger)
- Consumption based pricing for watsonx.data SaaS is listed below:

Capabilities  Price (USD) / Hour Cache optimized node cost per hour $2.80 ![](Aspose.Words.10f87835-25ca-4b31-ba66-2c96582179f7.005.png)

Computer optimized node cost per hour $6.50 

Supporting services per hour $3.00 ![](Aspose.Words.10f87835-25ca-4b31-ba66-2c96582179f7.006.png)

- In addition, the consumption will be based on notes and computing hours. For additional information please review our t-[shirt pricing deck .](https://ibm.seismic.com/Link/Content/DC4QGj6Q4Bjm487X6jp6dqm2QGqd) This deck is sized for a single cluster with performance characteristics. 

Find more information on p[ackaging and pricing on Seismic. ](https://ibm.seismic.com/Link/Content/DCJXVRXPCM3FB8cX3RWQQ4Pp6jdj)

What are the tier plans available for watsonx.data SaaS and what do they include?

- watsonx.data Saas is available with Trial, Standard, and Premium watsonx Tiers.
- Trial Tier: Standard Tier feature set
- Credits are limited to 30 days and/or a $1500 consumption cap whichever 

  occurs first   

- Standard Tier:  
- Hive metastore and Iceberg catalog
- Infrastructure manager and query editor
- Presto query engine and connectors
- Spark, Db2Wh, and Netezza integration
- No Tier fee at Launch (planned for $1,500/month in Q3). 
- Premium Tier: Currently in development. 
- Essentials Tier: Not planned. 
- Technical 

What features are planned in 2023 for watsonx.data?

Multiple Query Engines: Drive analytics costs down with lower cost compute and storage and fit-for-purpose analytic engines, including Presto and Spark, that dynamically scale up and down. 

Cost-effective storage: Watsonx.data uses simple, reliable object storage to store vast amounts of data at a fraction of the cost of traditional block storage. 

Single copy of data: Leverage open Apache Iceberg table format, metadata, and cost - effective object storage to share a single copy of data across multiple query engines for analytics and AI workloads. 

Built-in governance and security: Protect data, manage compliance, and maintain trust with built in-governance, access controls, and enterprise security. Integrate with IBM’s centralized governance capabilities to enable responsible, transparent and explainable data and AI workflows across the enterprise. 

Easy to use console: Load and access data across cloud or on-premises environments in minutes using a simple UX and console with full-service storage, engine, and meta store - all integrated and preconfigured.

Semantic automation: As a tech preview in 2023, we will demonstrate how to leverage AI for watsonx.data so users can easily discover, augment, and refine data for AI using self-service, conversational access. Similarly, users can leverage governed enterprise data in watsonx.data to seamlessly train or fine-tune wa[tsonx.ai founda](http://watsonx.ai/)tion models. 

watsonx.governance Specific Questions

- General 

What is watsonx.governance?

Watsonx.governance is the next-generation enterprise toolkit to govern AI workflows. It provides enterprises with three key capabilities to govern the entire AI lifecycle: lifecycle governance, risk management and regulatory compliance. Lifecycle governance provides the capability to monitor the AI lifecycle, including automated visibility of what data was used, how the model was built, and any variations on that model. Risk management facilitates the identification and management of risk at scale, and finally, regulatory compliance enables adherence to external AI regulations for audit and compliance purposes. 

How is watsonx.governance unique, first of a kind, or differentiating?

Watsonx.governance is unique in providing a solution that manages AI workflows, including AI regulation and risk management. This offering provides clients the basis for positioning AI outcomes as responsible.

As more businesses rely on AI models to execute business strategies, operational risk processes must be updated to assess risks related to using these models and ensure the appropriate controls are in place. Watsonx.governance ensures that model risk is understood at the front line of business operations. By aligning models to key business processes and applications, the organization can highlight the risks that arise from Model Development, Deployment and Usage directly with key business stakeholders. It’s a shift from model risk as a siloed view, to model risk in context. 

With watsonx.governance, organizations can efficiently conduct risk assessments, define controls to mitigate those risks, and continuously assess control performance. In addition to providing model risk governance, watsonx.governance  helps organizations manage operational risks using models supporting the business strategy. The 

application also includes the ability to manage regulatory requirements and associated controls to ensure compliance with AI legislation on both a model-by-model, and in aggregate approach. 

Firms aiming to provide consistent, trusted service to clients need to factor the growing reliance on AI into their resilience posture in the same way they refer to applications, physical assets, vendors, and cloud providers. Watsonx.governance allows them to leverage structured AI model risk assessments and AI model monitoring to ensure service delivery to clients and markets. 

What services/products are represented by watsonx.governance? What are the product components underneath watsonx.governance?

- OpenPages  
- Factsheets 
- OpenScale 

Are there any new offerings within the rebranded watsonx.governance portfolio, or are these largely pre-existing solutions that have been repositioned under the new “watsonx” naming convention?

Watsonx.governance is not a rebrand. There will be new capabilities, in addition to the capabilities currently provided by IBM AI Governance. 

When is the actual launch of watsonx.governance? If not until next year, will AI governance and data governance remain separate? 

The actual launch of watsonx.governance is scheduled for 4Q2023. AI and data governance will remain separate. As indicated in the definition, watsonx.governance is designed specifically for the governance of AI lifecycles.

Why would we announce watsonx governance at Think when it will not be available as a solution until next year?  

We announced watsonx at Think, 2023. Watsonx is a single subscription that provides users to access multiple AI capabilities including watsonx.governance. Consequently, the watsonx.governance announcement cannot be decoupled from the overarching watsonx announcement. Watsonx.governance will GA in 4Q2023. The announcement at Think will enable sellers to build pipeline ahead of the GA date.

For more details, refer to the wa[tsonx roadmap on Seismic for the](https://ibm.seismic.com/Link/Content/DCMmpHHmJchDq8qW3dM9TX8qjW9d) latest. 

Where can I learn more about watsonx.governance? Start here in [Seismic. ](https://ibm.seismic.com/Link/Content/DC2gJqq6D6TWRGWCQHGGHfTB2CXd)

- GTM 

Who is the intended user for this product/service?

The intended user is any client interested in governing their AI workflows for AI lifecycle, risk management and compliance to AI regulation. (Personas include risk managers, compliance and/or information officers, and data scientists).

Aren’t there different decision makers and stakeholders for Data and AI? Won’t combining these into a single solution cause sales and marketing challenges? 

There are multiple entry points for watsonx.governance opportunities. Sellers will be trained to understand the key personas (Chief Risk Officer for risk management, Chief Compliance Officer for compliance, Chief Data Office, Chief Information Officer, and Data Scientist for model governance).

When will watsonx.governance be available to clients? 

Watsonx.governance is planned for Generally Availability on IBM Cloud as-a-Service in November 2023. For more details, refer to the wa[tsonx roadmap on Seismic for the ](https://ibm.seismic.com/Link/Content/DCMmpHHmJchDq8qW3dM9TX8qjW9d)latest. 

Between the announcement of watsonx on May 9th and the eventual GA of watsonx.governance, how will we continue to position the existing data fabric use cases? 

After GA, AI governance will no longer be marketed as a data fabric use case since its capabilities will be part of watsonx.governance. Similarly, Data Science & MLOps will no longer be marketed as a data fabric use case since its capabilities will be part of watsonx.ai. All other data fabric use cases will be positioned as part of the architecture.

What are the migration paths for existing clients?

Migration paths will be determined after packaging for watsonx.governance has been finalized. 

Will clients have the flexibility to customize watsonx.governance for specific pain points, or are the use cases pre-determined by the watsonx.governance solution? Watsonx.governance solves a pain point associated with governing AI workflows. Clients will have the flexibility to use the watsonx.governance toolkit to address AI lifecycle governance, risk management and compliance with AI regulation.

What are our routes to market?

Our routes to market include Data and AI sellers, IBM business partners, the Amazon marketplace, and digital self-service.  

What will a client use watsonx.governance for? Can you provide 2-3 use cases or examples? 

Yes, OpenPages provides out-of-box workflows to help manage:

Inventory + Lifecycle Management

- Model inventory to track key information
- Model candidate workflow 
- Model development workflows to review and approve new models
- Model attestation and related workflow with configurable questions
- Model decommissioning workflow to track the retirement of models no longer 

  used 

Risk Assessment + Model Validation

- Model risk scorecard methodology and related workflow to determine model tier
- Conduct reviews (validation) of new and existing models and document fieldwork, challenges, and approvals

Performance Monitoring 

- Dashboards to give executives a view into the status of the entire inventory of models and provide actionable insights at a glance
- Document metrics and track metric values over time

Change/Issue Management 

- Track issues and incidents related to models in OpenPages included Issue Management Solution 
- Workflow to document and approve changes to models

Who are the key competitors we are targeting with this solution, and how is IBM's solution better for clients?  

[Trustible.ai i](https://www.trustible.ai/)s a new offering, but they don’t have OpenScale or FactSheets functionality. They are going to market with a similar governance-in-process value proposition. [Trustible.ai a](https://www.trustible.ai/)nd [Monitaur.ai are](https://www.monitaur.ai/products) focused on GovernML and RecordML. 

Are we targeting specific industries with this solution? If so, which ones and why? Watsonx.governance is applicable to any organization and/or industry that leverages AI and requires governance of AI workflows. This is a cross-industry solution. 

- Packaging/Sizing 

Will watsonx.governance replace the existing data fabric use cases including data governance and data integration?

No, watsonx.governance is a component of the broader watsonx platform. It is very specifically geared for clients interested in governing AI workflows. Some of the capabilities of the AI governance use case will be incorporated into watsonx.governance. Similarly, some of the capabilities of the Data Science & MLOps use case will be incorporated into watsonx.ai. The remaining data fabric use cases will continue to form the architecture for a data foundation that delivers the right data for AI workflows. 

Is OpenScale part of watsonx.governance only, or also under watso[nx.ai? If the ](http://watsonx.ai/)former, are there any changes to the IBM Data Science & MLOps Express offering? OpenScale will only be a part of watsonx.governance, not watsonx.ai. No immediate changes are planned for the Data Science & MLOps Express offering (see previous answer).  

If watsonx.governance is positioned as the lead offering, how do we position the non - governance capabilities (e.g. data integration, data replication, data observability, master data management, etc)?

Watsonx.governance is the next-generation enterprise toolkit to govern AI workflows. The non-governance capabilities will continue to be a part of the data fabric architecture that enables a data foundation that delivers the right data for AI workflows.

Sales Specific Questions 

Audience: IBM Sales leads Purpose: Seller enablement 

When will this change be effective for sellers/partners/clients?

The change will be effective at the GA of watsonx.ai and watsonx.data in July, with watsonx.governance coming later in the year.

Where do we go for more information?

[Seismic i](https://ibm.seismic.com/Link/Content/DCTGRDXWbFqR6G7Wm7pMjjD4V27j)s continually updated with the latest client-friendly content. Internal comms and help will be available o[n the w3 publisher site. ](https://w3.ibm.com/w3publisher/watsonx)

Seismic: [https://ibm.seismicSeismicnk/Content/DCTGRDXWbFqR6G7Wm7pMjjD4V27j ](https://ibm.seismic.com/Link/Content/DCTGRDXWbFqR6G7Wm7pMjjD4V27j)Product/Dev publisher site: htt[ps://w3.ibm.com/w3publisher/watsonx](https://w3.ibm.com/w3publisher/watsonx)

Is there early access for IBMers to try watsonx? i.e., use it to create realistic code? [Watsonx.ai can be used here](https://bam.res.ibm.com/)

[Watsonx.data can be used here](https://ibm.seismic.com/Link/Content/DC3mhFXPVf6jhGHJqTR3PXc4mGp8)

What does the ‘x’ in watsonx stand for?

It stands for scale.  IBM seeks to help clients to scale AI across their business by leveraging Generative AI technology.

What is the Unique Selling Point of IBM Foundation Models vs other providers' Foundation Models? 

We've curated our foundation models, so we don’t simply dump everything in one place and hope for the best! 

How can I tag a watsonx opportunity correctly in IBM Sales Cloud?

Each watsonx component has a specific UT30. Type in “watsonx” in the search bar for product identification and you will see a drop-down of options. Seismic also contains of specific ISC guidance assets per component. (Note: watsonx.governance won’t be visible before 07/11)

What is IBM Consulting doing in the generative AI space, and how are they leveraging watsonx?

Visit the I[BM Consulting Lighthouse Space to ](https://w3.ibm.com/services/lighthouse/spaces/view/generative-ai-for-ibm-consulting/overview)learn about their 'watsonx everywhere' selling campaign, their point of view on generative AI and their approach to this space.

How do I connect with an IBM Consulting colleague who might be talking to my client about watsonx or generative AI? 

Visit this[ Lighthouse page wh](https://w3.ibm.com/services/lighthouse/spaces/view/generative-ai-for-ibm-consulting/watsonx-everywhere-market-contacts)ich is regularly updated, and shows you the IBM Consulting leads for watsonx in each market.

What is the list of the available Slack Channels available for watsonx.

- [#Watsonx-ai-enablement ](https://ibm-analytics.slack.com/archives/C057G8L357W)
- [#watsonx-sales-oppty  ](https://ibm-cloud.slack.com/archives/C058N36776H)
