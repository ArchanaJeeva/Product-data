FAQ: Positioning IBM’s Generative AI Offerings

**What are IBM’s Generative AI offerings?**

IBM’s Generative AI Offerings are structured around three key product areas:

1. **AI Assistants** that are specifically built and designed to address targeted Generative AI workflows in specific lines of business (LOBs).
1. An **AI and Data Platform** that empower enterprises with the tools to leverage Gen AI across their organizations, with the best of open source tools and trusted model.
1. Embedded Generative AI in existing IBM products, enhancing and extending the value proposition that new and existing customers

**AI Assistants:** 

AI assistants are GenAI applications powered by watsonx. They help to automate workflows and implement AI across a variety of business and technical functions such as customer service, HR and code development, key products include: watsonx Assistant, watsonx Orchestrate, watsonx Code Assistant, and watsonx BI Assistant. 

**AI & Data Platform:** 

The AI and Data platform includes three core components, watsonx.ai, watsonx.data, and watsonx.governance, designed to help enterprises scale and accelerate the impact of AI with trusted data, open AI, and targeted tools across their firms, that empower clients to confidently embrace GenAI. 

Enterprises are turning to watsonx because watsonx is:

- **Open**: Based on open technologies that provide a variety of models to cover enterprise use cases and compliance requirements.
- **Targeted**: Targeted to specific enterprise domains like HR, customer service or IT operations to unlock new value.  
- **Trusted**: Designed with principles of transparency, responsibility and governance so you can manage legal, regulatory, ethical and accuracy concerns.
- **Empowering**: Go beyond being an AI user and become an AI value creator, owning the value your models create. 

**What is the relationship between watsonx.ai and the AI Assistants?**watsonx.ai and the AI Assistants all use AI models to help clients leverage GenAI to do their jobs faster, more efficiently, more repeatably, and with fewer errors.  

Whereas watsonx.ai allows clients to work with generative AI models directly, training, tuning, managing and customizing them for their particular use cases, the AI Assistants are already pre-tuned for specific tasks such as accelerating COBOL code modernization to Java in the case of watsonx Code Assistant for Z, or further increasing containment rates in the contact center using watsonx Assistant. In both cases, watsonx.ai is often helping support those GenAI use-cases “under the hood” within the AI Assistant, but is not directly exposed to the client as a tool for the end-user.  

**Regarding the Q2 2024 open source announcements, does this mean watsonx Code Assistant, or other AI Assistant products are now open source?** 

No. Only select Granite series models and InstructLab are being open sourced. Our AI Assistant products, like watsonx Code Assistant and watsonx Orchestrate, are not being open sourced. Instead, these AI Assistants will benefit from some of the model improvements driven by InstructLab engagement by the community. Domain specific models, like the models in watsonx Code Assistant for Z, are not being open sourced at this time.

**What does this mean for IBM watsonx.ai if we are giving the models for free?** 

IBM watsonx.ai is much more than just an access point for IBM proprietary models. IBM watsonx.ai serves as a studio for building end-to-end AI solutions. Offering a variety of model options, we proudly continue to serve our IBM Granite series, including open source and custom variants. 

The models being open sourced are not customized or domain specific. Proprietary, domain specific language models will continue to be in watsonx products, along with open source models and third - party models – like Llama and Mixtral. An example of a domain-specific language model is IBM Granite Multi-Lingual 20B, which is not being open sourced in this announcement.

**Now that we have open sourced IBM’s Granite models, will IBM keep developing Granite models? Or will all development be driven by the community?** 

Yes, IBM will continue to develop Granite models. For both open source consumption, and as differentiators in our Gen AI products, we will continue to develop and invest in our Granite models. For example, our Granite Japanese, Granite Multi-Lingual, and Cobol-specific versions of the Granite Code model in watsonx code Assistant are all proprietary models that will continue to be developed within IBM.  

FAQ: Positioning IBM and Red Hat in Generative AI 

**What are IBM and Red Hat’s Generative AI offerings? What is the high level positioning for each?**

**Red Hat Enterprise Linux AI (RHEL AI):**  

RHEL AI is a single-server, non-High-Availability (HA) offering, primarily targeted for individual 

developers or small teams, and oriented towards GenAI production use cases that do not require multi - system deployment of scaling workloads. RHEL AI will be embedded inside of Red Hat OpenShift AI (RHOAI). 

**Red Hat OpenShift AI (OpenShift AI)**:**  

OpenShift AI in turn adds High Availability capabilities, and model lifecycle management (i.e., model serving, training, etc.) across containers, to RHEL AI. OpenShift AI has been embedded within watsonx.ai.  

**watsonx.ai**:**  

IBM watsonx.ai adds access to a variety of both open source and proprietary models (such as Llama 3, Mistral, other popular 3rd party models), an enterprise-ready studio and other tooling for building end - to-end AI solutions, including out-of-the-box integration with other watsonx products, and other enterprise AI capabilities designed to help scale generative AI. IBM watsonx.ai helps make the 

inferencing engine and scale provided by Red Hat accessible to enterprise applications, workflows, and tools.  

**What personas or buyer types should sellers & marketers focus on for each offering?** 

**RHEL AI**:  

Development Manager who wants to enable their team to experiment with InstructLab and the Granite model (and other models) locally on their systems to prototype useful GenAI solutions for their organization. 

AI Developers who evaluate, develop, tune, optimize, and deploy Generative AI models. **OpenShift AI**:   

DevOps Manager who wants to deploy a GenAI solution with high availability at scale across hybrid cloud, via containers run on Red Hat OpenShift.

AI Engineers who build end-to-end workflows and deploy in production at scale, evaluate the technical infrastructure, and focus on optimization and integration into existing frameworks or platforms.

Data Scientists/Data engineers who are responsible for designing and building data pipelines, model training and tuning. 

AI App Developers who create Generative AI infused software applications by integrating foundation models and AI algorithms.

**watsonx.ai:**  

VP of Data & AI who wants to ensure that all GenAI solutions are developed in a consistent, repeatable, auditable, verifiable, and explainable way across their entire lifecycle and across the whole enterprise

Line of Business Leader who wants to broadly leverage AI across both their technical and business communities in the broadest manner.   Interested in all aspects of the AI lifecycle including AI, Data management and Governance.  Inclusive of broadest constituents LOB App Dev, Business Analysts, Compliance leaders, Data Owners and DevOps leads.  

In addition, the personas relevant for OpenShift AI would also be applicable to watsonx.ai.

**What is the technical relationship between Red Hat’s offerings and IBM’s? When will watsonx.ai be integrated with OpenShift AI?**

IBM watsonx.ai is available today, and provides access to (optionally installable) Red Hat OpenShift AI.  With watsonx.ai v2.0 release at the end of H1 2024, watsonx.ai will embed OpenShift AI to replace the current infrastructure layer and OpenShift AI will become a technical pre-requisite for the Foundation Model capabilities of watsonx.ai.

- At present, clients can install OpenShift AI using the following instr[uctions.  In futu](https://cloud.ibm.com/docs/openshift?topic=openshift-datascience)re releases (targeted for watsonx.ai version 2.0), OpenShift AI is a prereq installed before watsonx.ai deployment
- watsonx.ai 2.0 will support all the features of OpenShift AI

Separately, Red Hat will launch RHEL AI in H2 2024, after which point, RHOAI will embed RHEL AI, meaning that watsonx.ai will both commercially and technically embed RHOAI, which will embed RHEL AI.  

**If a client is interested in a Red Hat offering like OpenShift AI, why would they seek watsonx.ai?** 

IBM watsonx.ai addresses the needs of technical and line-of-business user roles in a single collaborative studio interface to support end-to-end AI workflows. This allows users and teams to work with and scale generative AI, beyond what could be accomplished directly in OpenShift AI.  

Furthermore, watsonx.ai offers integration with watsonx.data and watsonx.governance, supporting a client’s complete enterprise AI/ML lifecycle.

**What models are being open sourced and will be included in RHEL AI?**

Red Hat is open sourcing IBM Research Granite code models (3B, 8B, 20B, and 34B models), as well as the Granite 7B English model.

**What Red Hat offerings will include these new open sourced capabilities?** 

Red Hat OpenShift AI (OpenShift AI), which has been in the market since 2023, and the new Red Hat Enterprise Linux AI (RHEL AI), to be released in H2 2024, will include the Granite code and Granite 7B English models.  

**Are there capabilities – coming from OpenShift AI or RHEL AI - that should be positioned in a watsonx.ai deal?**

Yes.  Key capabilities from Red Hat embedded in watsonx.ai include:

- Through the [InstructLab project, part](https://huggingface.co/instructlab) of RHEL AI, Red Hat and IBM have released select open source licensed Granite language and code models that are supported and indemnified by both companies. Now, developers can collectively enhance the IBM Granite code models (3B, 8B, 20B, and 34B models), in addition to the previously open sourced Granite 7B English model with new skills and knowledge, just as they would contribute to any other open source project.
- Managing and tuning the deployed High Availability (HA) AI environment with OpenShift AI.  Includes model serving and model monitoring, and hardware acceleration.

FAQ: Sales, Client, and Deal Progression

**Does Red Hat’s announcements around RHEL AI or OpenShift AI affect IBM’s sales motion at all?** 

No. There is ***no change or impact to any deals or sales motions*** related to this announcement. These capabilities are not planned to GA until H2 2024. IBM sellers should continue working closely with leadership at clients and partners to develop use cases that leverage and deploy the watsonx platform and AI assistants. What this announcement unlocks for IBM and Red Hat is greater awareness and buy - in at the developer level, which can help accelerate our existing motion.

Additionally, watsonx.ai users will continue to have access to all of the Granite foundational models, which are available on H[ugging Face and](https://huggingface.co/ibm-granite) included in Red Hat's products. 

Red Hat will maintain its commitment as a leading provider of open source technology, serving as the foundation of our AI tech stack. Meanwhile, watsonx will differentiate itself by focusing on enterprise capabilities and innovation higher up the AI tech stack. This strategic partnership and distinct positioning will enable us to accelerate our joint go-to-market and support the ambitious watsonx growth targets. 

**My client/partner has already purchased watsonx.ai. Do announcements around opensource, RHEL AI or OpenShift AI impact my customer at all?** 

No, nothing changes for existing customers. Over time, watsonx.ai will embed OpenShift AI and RHEL AI, but no change from an entitlement or deployment perspective. 

**Do these announcements involve any changes to existing incentives for watsonx for IBMers?** 

There is no change to incentives. Access detail on incentives and sales plans on Sales In[centives Workplace. ](https://w3.ibm.com/w3publisher/global-sales-incentives/incentives-workplace)

**How does seller compensation for RHEL AI, OpenShift AI, and watsonx.ai work?**

Currently, IBM sellers are paid on watsonx.ai and Red Hat sellers are paid on RHEL AI and OpenShift AI. In addition, Red Hat sellers are also paid on the OpenShift AI component within watsonx.ai as follows:

- Red Hat sales teams and leadership will receive ACV+Cloud and ARR attainment against their respective plans based on the revenue share which is allocated to Red Hat (16.63%)
- ACV+Cloud: The revenue share for Red Hat products will receive a **2.5x multiplier** to bring attainment near the average sale price of OpenShift and OpenShift AI
- Red Hat sales teams should not forecast any IBM offerings
- ARR application is a work in progress and more information is forthcoming for Red Hat sellers

**Between IBM and Red Hat, who can sell which product, and how does co-sell or lead-passing work?** 

IBM sellers will be the ones executing the sales for watsonx.ai. However, it is important for Red Hat sellers to help IBM sellers understand the client/partner landscape related to Red Hat OpenShift and OpenShift AI.  Red Hat sellers will receive compensation for each watsonx.ai sale per the guidelines discussed above.

**Where can I learn more about our “rules of engagement” for selling with and alongside Red Hat?**

The recent announcement does not change the sales focus of RedHat and IBM.  Both sides can execute sales motions into their respective customer bases, with their branded products (i.e. IBMers selling IBM products, Redhatters doing with same with Red Hat products).  

It is recommended that sellers work together and develop a strategy that addresses customer goals, needs and roles in various parts of the enterprise that will be consumers of AI.  If IBM and Red Hat sales approaches are not in synch, there may be confusion which could have been avoided by a common view of the customer and the solution.

In some cases it will make sense for IBM and RedHat to work independently addressing goals by targeting Developer, MLOps and Data Owners, Enterprise or Business roles with the unique offerings that best fit these roles.  This approach may be better at addressing immediate needs and smaller consumer communities and fast targeted start-up seeding AI consumption.

In some cases it will make sense to focus on addressing customer needs and the identified roles with a single offering – with the ability to extend to AI oriented data management and governance as well.  This approach limits complexity and provides the customer the broadest solution, most flexibility, addresses most user roles and provides highest ROI.    

Rules of engagement:

1. Be open in the approach that best addresses the customer needs
1. Be strategic in building out a strategy and execute with a target in mind
1. Work together and communicate as a team
1. If conflicts or differences in alignment arise, escalate to sales management for help
1. In all cases view the RedHat and IBM solutions as an integrated offering, and communicate that, and show that, to the customer  

In the short term, SSPs and SSAs should notify the AI BU of any in-flight opportunities that they consider may be at risk of losing significant revenue for lack of alignment between IBM and Red Hat sellers. This includes questions about technical capabilities. 

**How can Red Hatters and IBMers benefit from engaging with each other?** 

Sellers across both IBM and Red Hat should work with each other to build joint pipeline and close early deals together immediately. 

The account planning exercise for both strategic and non-strategic accounts should consider both client/partner options:

- The inclusion of watsonx.ai, OpenShift, OpenShift AI, and RHEL AI as a combined offering
- The inclusion of watsonx.ai and Red Hat offerings as standalone offerings that form toolset to embed AI at scale 

IBM team members should engage with their Red Hat counterparts where possible. This strategy is a joint effort and only through deep collaboration and communication will we achieve optimal outcomes.

**How does Red Hat nominate a potential client/partner to IBM?**

Watsonx.ai, OpenShift, OpenShift AI, and RHEL AI opportunities should be discussed and mapped during the joint account planning process between RH & IBM sales personnel. If a Red Hatter is not in contact with their IBM peer, please reach out to the Geo Alliance IBM Leader for more information.

**Are IBM sellers able to provide more competitive pricing on Red Hat products than Red Hatters?** 

No. The go-to-market dynamics for this partnership establishes a consistent purchasing flow that maintains the value in our offerings regardless of how the direct sale is initiated. IBM sellers will sell IBM products and Red Hat sellers will sell Red Hat products. 

**Will we have trade-up part numbers to move clients from RHEL AI or OpenShift AI to watsonx.ai?**

No but we do have specific parts that have built in discount and leverage the RHEL AI (planned)  and OpenShift AI entitlements.  

**What training and badging are available for each product?**

IBMers can find training and badging for watsonx products on Se[ismic ](https://ibm.seismic.com/Link/Content/DCGX2M377qBM38TMpQ7DB3WVmQg8)Cross-training across Red Hat and IBM teams is TBD. 

**How does Red Hat commercialize its offerings?** 

Red Hat sellers monetize OpenShift AI today, and RHEL AI in the future, through subscription entitlements. However Red Hat sellers do get credit for sales that include embedded Red Hat offerings executed by IBM. 

**How is RHOAI licensed within watsonx.ai? Are there restrictions or limits on how RHOAI is used with watsonx.ai?**

watsonx.ai entitles clients to unrestricted use of RHOAI, at a ratio of 1 watsonx.ai VPC = 1 RHOAI core (e.g. a purchase of 100 watsonx.ai VPCs would allow clients use of 100 cores of RHOAI). See IB[M Terms for the explicit language on watsonx.ai terms.](https://www.ibm.com/support/customer/csol/terms/)

**What does the entitlement of RHOAI in w[atsonx.ai allow](http://watsonx.ai/)? What are the restrictions or limitations on usage?**

watsonx.ai includes technically unrestricted OpenShift AI. This allows:  

- A single, salable package to meet enterprise customer needs
- Deployable as  
- either a purely open source based RHOAI environment that a developer or low - level focused data scientist would enjoy, 
- or as a full enterprise watsonx.ai with capabilities dependent on RHOAI as a technical pre-requisite 
- with no incremental transaction or commercial friction in moving between the two

IBM watsonx.ai’s license terms clearly delineate that entitlement to 1 watsonx.ai license VPC is equivalent to 1 RHOAI core ([link to the terms, exac](https://www.ibm.com/support/customer/csol/terms/?id=L-MNZL-NFMSHF&lc=en)t language below). 

Other FAQ 

**Where can I learn more?** 

- Sales Kits & other Seller info 
  - [watsonx.ai ](https://ibm.seismic.com/Link/Content/DCJH7MbqmMBmG8MPFjm2jWWfjgbP)
  - watsonx Assistant 
  - watsonx Orchestrate
  - watsonx Code Assistant
  - [Sales Incentives Workplace](https://w3.ibm.com/w3publisher/global-sales-incentives/incentives-workplace)
- For Red Hat and IBM rules of engagement information, please work with your sales leadership.
- Model Information
  - [IBM Granite on Hugging Face](https://huggingface.co/ibm-granite)
  - IBM Granite Research [generative AI models ](https://huggingface.co/ibm/granite-7b-base)
- Capabilities 
  - InstructLab overview deck for sharing with clie[nts and partners in Seismic, as well ](https://ibm.seismic.com/Link/Content/DCbjQQbF6FWpH87M3V2R3JPcMBfd)as an [internal FAQ a](https://ibm.seismic.com/Link/Content/DCCgJ8ppTH6438FRp4MC6fcbbD2P)nd i[nternal blog ](https://w3.ibm.com/w3publisher/watsonx/blogs/82b09ae0-fda4-11ee-9ddc-c3a5a328de98)
  - [InstructLab resource page](https://w3.ibm.com/w3publisher/ai-for-business/instructlab)
- Other
  - [AI for Business blog ](https://w3.ibm.com/w3publisher/ai-for-business/momentum-blog/b6ad2b90-089b-11ef-b6f3-89ed82bc1da3)

**What was announced in Q2 2024 in the IBM and Red Hat partnership, around Generative AI?** 

There were three key announcements from the May 2024 Red Hat Summit:

- Open sourcing of select **Granite language and code models** that are fully supported and indemnified by Red Hat. 
- **A supported, lifecycle distribution of InstructLab** that provides a scalable, cost-effective way to enhance LLM capabilities and make knowledge and skills contributions accessible to a much wider range of users.
- Red Hat’s **complete enterprise support and lifecycle promise** that starts with a trusted enterprise product distribution, 24x7 production support, extended model lifecycle support and model intellectual property indemnification.

For more information on Red Hat’s offerings and what is being announced, read the press rel[ease. More ](https://www.redhat.com/en/about/press-releases/red-hat-delivers-accessible-open-source-generative-ai-innovation-red-hat-enterprise-linux-ai)details on watsonx.ai and InstructLab can be found in the watso[nx.ai sales kit, including](https://ibm.seismic.com/Link/Content/DCJH7MbqmMBmG8MPFjm2jWWfjgbP) a client dec[k, ](https://ibm.seismic.com/Link/Content/DCbjQQbF6FWpH87M3V2R3JPcMBfd)and [InstructLab resource page.](https://w3.ibm.com/w3publisher/ai-for-business/instructlab)
Page 10 
