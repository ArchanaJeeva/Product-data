**Evaluation Warning : The document was created with Spire.Presentation for Python**

**watsonx![](Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.001.png)![](Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.002.png)**

Synthetic data generator

Competitive overview 

*Updated Dec 21st, 2023*

Summary

Startup vendors have a head-start relative to IBM’s Synthetic data generator service on watsonx, providing users with the ability to quickly and easily generate high-quality synthetic tabular data, reports to evaluate the data’s quality, and tools to minimize data privacy risk when using existing, sensitive data. 

In the 1H 24, IBM expects to make significant progress in closing these gaps (evaluation metrics, differential privacy, and potentially a generative-AI model) , which should make the solution more competitive in the 2H 2024.

Until then, our differentiators are the scope & expertise of IBM and the access to foundation model LLMs via the broader watsonx.ai platform.   Currently, we’re actively working with several clients (see Slide 4) on validating and using an early version of the generative-AI model to be released in Q2 24. 

![](Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.003.png)

**Evaluation Warning : The document was created with Spire.Presentation for Python**

Feature comparison

![](Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.004.png) Have feature ![](Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.005.png) Partial ![](Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.006.png) Don’t have ![](Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.007.png) Unknown



|**Category**|**Features**|**Synthetic Data Generator**|**Hazy**|**Mostly.ai**|**Gretel**|**Tonic**|
| - | - | - | - | - | - | - |
|**Data needs**|Use existing data||||||
||Custom data schema||||||
|**Data types**|Categorical||||||
||Continuous||||||
||Date/time-series||||||
||Spatial/geo-location Special data types||Unknown|Unknown|Unknown|[Link](https://docs.tonic.ai/app/generation/generators/generator-reference)|
||Unstructured text|via watsonx.ai LLMs|||||
||Images||||||
||Videos||||||
|**Model types**|Rule-based||||||
||Statistical||||||
||Generative-AI|Q2,’24|||||
||Agent-based simulations|Q4, ’24|||||
||Foundation models|via watsonx.ai LLMs (unstructured only)|||[Early access ](https://gretel.ai/tabular-llm?utm_source=tldr-ai&utm_medium=newsletter-sponsorship&utm_campaign=tabular%20llm&utm_content=tldr-20230829)(tabular FM)||
|**Core features**|Validation reports|Q1, ’24|||||
||Referential integrity|Q2, ’24|||||
||Database connectors||||||
||Privacy|Q1, ‘24|DP|Not differential, but PbD|DP|DP|
||Subsetting|No timing|Unknown|Unknown|Unknown||
||Masking|Anonymization only||||Multiple approaches|
|**Deployment**|SaaS||||||
||Onprem||||||

6
**Evaluation Warning : The document was created with Spire.Presentation for Python** 

**IBM overview ![](Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.008.png)![](Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.009.png)**watsonx.ai 

IBM, watsonx.ai 

*The Synthetic data generator service on their watsonx.ai platform  generates structured tabular data from existing data or a custom data  schema using a variety of models (only 1 model yet available)* 

10
**Evaluation Warning : The document was created with Spire.Presentation for Python** 

**General info Use cases & customers![ref1]**

Website: [www.watsonx.ai](http://www.hazy.com/) Use cases

- AI model training
- Demo data
- Data for internal training
- Edge case data

  Customers

- No production customers
- Early pipeline: Bradesco, Global Payments, Goldman Sachs, Wells Fargo, DATEV, Itau

**Strengths**

- IBM has vertical industry experience & professional services with broader integrations with platform![ref2]
- Enterprise-grade features with multiple connectors
- LLM foundation models available, as well as governance

**Weaknesses**

Missing key features, relative to competitors and user needs![ref3]

- Time-series
- Referential integrity
- Validation reports
- Data privacy mechanism
- Gen AI model

See roadmap for when these will be available

11
**Evaluation Warning : The document was created with Spire.Presentation for Python** 

**Competitive overview** 

Startups ![ref4]![](Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.014.jpeg)

Hazy 

*Focus on synthetic data generation for highly regulated large enterprises  with legacy architecture. Self-proclaimed first company to take synthetic  data to market as a viable enterprise product, with links to academics  from the Alan Turing Institute and a few published research papers* 

13
**Evaluation Warning : The document was created with Spire.Presentation for Python** 

**Competitive overview** 

**General info  Use cases & customers![ref1]**

Use cases - Data sharing, AI/ML dev, UK-based Testing and product dev, Fairness 

and explainability; Telco, Banking, Website: [www.hazy.com](http://www.hazy.com/) Insurance specific use cases

Customers:

Vodafone, BMW, Wells Fargo, Nationwide, PwC, Accenture, NatWest, 

**Strengths**

- Leader in generating synthetic data for financial services![ref2]
- Significant public material explaining the privacy-utility tradeoff
- Incorporates data governance
- Strategic partnership investment from Microsoft
- Core features and data types: time -series, referential integrity, gen- AI model, privacy reports, differential privacy

**Weaknesses**

Lacks breadth and depth of IBM’s experience across software, services, hardware, and various industry verticals![ref3]

No agent-based simulation for mature enterprises

14
**Evaluation Warning : The document was created with Spire.Presentation for Python** 

**Competitive overview** 

Startups ![ref4]![](Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.015.jpeg)

Mostly.ai 

*Mostly AI develops and offers asyntheticdataengine that provides  organizations the ability to generate realistic and  representativesyntheticusers anddata, retaining structure and  variation while preserving privacy.* 

16
**Evaluation Warning : The document was created with Spire.Presentation for Python** 

**Competitive overview** 

**General info ![ref1]**

Founding year: 2017, Austria Website: [www.mostly.ai ](http://www.mostly.ai/)Funding: $31M total funding 

**Use cases & customers** 

Use cases - Data sharing, AI/ML dev,  ![ref2]Testing and product dev, Fairness  and explainability; Telco, Banking,  Insurance specific use cases 

Customers: 

Citi, City of Vienna, Erste, Merkur,  Telefonica,  

**Strengths Weaknesses**

- Core features available around quality  Doesn’t deploy differential privacy, reports, privacy measures, referential ![ref3] which is the only mathematical integrity, time-series, and gen-AI  guarantee of privacy

  model (GAN-based)

- Offers integrated solution with  Smaller and lacks enterprise and support for cloud & on-prem solutions industry experience 
- Offers community & enterprise 

  products

- Professional services & GPU support
- Scalable deployment via Openshift/Kubernetes containers

17
**Evaluation Warning : The document was created with Spire.Presentation for Python** 

**Competitive overview** 

Startups ![ref4]![](Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.016.jpeg)

Gretel 

*Gretel.ai was founded on a privacy-first mission to equip developers with  the ability to unlock innovation through safe, efficient collaboration with  sensitive data. …Gretel created easy to use, accessible APIs for  developers and data practitioners to generate high quality synthetic data,  classify and label, and transform and anonymize data* 

20
**Evaluation Warning : The document was created with Spire.Presentation for Python** 

**Competitive overview** 

**General info ![ref1]**

Founding year: 2019, USA Website: [www.gretel.ai ](http://www.gretel.ai/)$65.5M total funding 

Partnership withGoogle  Colaboratory to create artificial  data  

**Use cases & customers Strengths Weaknesses**

Use cases – deep learning ML for  Community/developer focused text or tabular, democratize data ![ref2]![ref3] • Potentially biggest footprint industry agnostic synthetic data market rather than enterprise-grade

access; finance and life sciences 

- Well-developed API 

industry uses

- Large number of customer use cases 

Customers: Illumina, SAP across industries (HSBC, Illumina, 

etc.)

- Multiple models to support various 

  synthetic data types: tabular, image, 

  text, and relational, time-series

- Core features: Referential integrity, 

  Gen-AI approach (LSTM nueral 

  network), differential privacy, quality 

  reports

21
**Evaluation Warning : The document was created with Spire.Presentation for Python** 

**Competitive overview** 

Startups ![ref4]![](Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.017.jpeg)

Tonic 

*Tonic.ai automatically creates **mock data** that preserves characteristics  of secure datasets so that developers, data scientists, and salespeople  can work without breaching privacy. The company provides data that is  modeled from a client's production data to help tell an identical story in  the client's testing environments.* 

23
**Evaluation Warning : The document was created with Spire.Presentation for Python** 

**Competitive overview** 

**General info Use cases & customers![ref1]**

Founding year: 2018, USA Use cases - Accelerate CI/CD 

lifecycle, Test dev; Retail, Health/ Website: [www.tonic.ai](http://www.tonic.ai/) wellness, Insurance industry 

specific uses

$43M total funding

Customers: ebay, Motley Fool, NHL, Flexport, Alegeus

**Strengths Weaknesses**

Core features: referential integrity,  Smaller and lacks enterprise and generative AI models, subsetting, ![ref2]![ref3] industry experience 

time-series, differential privacy, and 

onprem & Cloud deployments

Marketing focused on test data, but can handle AI use cases as well

Robust masking techniques (encryption, JSON masking, scrambling)

24
**Evaluation Warning : The document was created with Spire.Presentation for Python**

**Competitive overview**

Major players

25
**Evaluation Warning : The document was created with Spire.Presentation for Python**

**Competitive overview**

Major players are either using synthetic data or funding 3rd party solutions

 

|**Vendor**|**Product or Partnership**|**Use cases or Vendor’s usage**|**Key Aspects**|
| - | - | - | - |
|**Microsoft** |Open-source Synthetic Data Showcase, an automated pipeline for generating both synthetic and aggregate datasets that conserve the utility of the original, along with dashboards for |Synthetic Data Showcase started as a project within our[Tech Against Traffickinginitiative,](https://techagainsttrafficking.org/) and we believe that its ability to improve the |<p>- Full K-anonymity</p><p>- Dashboards</p><p>- Open-source</p>|
||visualizing and exploring these derived datasets. Generates |representation of at-risk groups can help us solve |• Automated pipeline|
||synthetic data to preserve privacy when sharing and analyzing |pressing societal problems and build a more |• Structured|
||sensitive datasets. The synthetic and aggregate data are |resilient world.||
||automatically loaded into a Power BI interface for interactive, |• Combatting trafficking with synthetic data||
||privacy-preserving data exploration.|• Protecting vulnerable groups in datasets||
|||• Synthesizing data with full k-anonymity||
Microsoft’s[Visual Studio Premiumalso](https://docs.microsoft.com/en-us/previous-versions/visualstudio/visual-studio-2010/dd193262\(v=vs.100\)?redirectedfrom=MSDN) has a built-in test data  • Application testing generator for Application testing


**Evaluation Warning : The document was created with Spire.Presentation for Python**

**Competitive overview**
|**Informatica**|Informatica® Test Data Generation automates the process of generating synthetic data for application testing. IT can set |<p>- Application testing</p><p>- Ensure applications function dependably </p>|<p>- Support for Tables</p><p>- Support for business </p>|
| - | :- | - | - |
||multiple relational and conditional rules to rapidly generate large |• Outsource testing and/or development without |rules|
||synthetic data sets containing both data errors and inconsistent |exposing production data to unauthorized users|• Structured |
||characteristics to simulate real-life scenarios. Data privacy is |||
||protected by creating synthetic data sets that mimic production |||
||data while not exposing it. |||
|**Google** |Partnership with[Gretel Syntheticsand ](https://github.com/gretelai/gretel-synthetics)Google[Colaboratory’s ](https://colab.research.google.com/notebooks/intro.ipynb)free GPUs to train a machine learning model to automatically |• [Google’s Waymo ](https://venturebeat.com/2020/05/20/waymo-is-using-ai-to-simulate-autonomous-vehicle-camera-data/)uses synthetic data to train its autonomous vehicles|<p>- Anonymized</p><p>- Python SDK</p>|
||generate fake, anonymized data with[differential privacy](https://en.wikipedia.org/wiki/Differential_privacy)guarantees.||<p>- Structured</p><p>- Unstructured</p>|

**Amazon** • [Amazon used synthetic datato ](https://www.amazon.science/blog/tools-for-generating-synthetic-data-helped-bootstrap-alexas-new-language-releases)train Alexa’s  ![](Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.018.png)![](Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.019.png)![](Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.020.png)![](Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.021.png)

language system in new languages 

- [Amazon Go](https://venturebeat.com/2019/06/05/amazon-go-uses-synthetic-data-to-train-cashierless-store-algorithms/)used synthetic data to train  cashierless store algorithms 
- Amazon helped launch workshop on synthetic  data generation to unite communities  investigating synthetic data generation to  improve machine learning and protect privacy. 

31
**Evaluation Warning : The document was created with Spire.Presentation for Python**

![](Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.022.png)

[ref1]: Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.010.png
[ref2]: Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.011.png
[ref3]: Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.012.png
[ref4]: Aspose.Words.7292de7a-47ac-4918-ad17-10cfd38eb0f7.013.png
