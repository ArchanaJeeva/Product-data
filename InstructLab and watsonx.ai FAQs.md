watsonx.ai InstructLab FAQs![](Aspose.Words.8d9ac787-8e37-495e-8d66-5a7693969639.001.jpeg)

April 18, 2024

IBM and Business Partner Internal use only

watsonx.ai![](Aspose.Words.8d9ac787-8e37-495e-8d66-5a7693969639.002.png)

Seller guidance  ![](Aspose.Words.8d9ac787-8e37-495e-8d66-5a7693969639.003.png)![](Aspose.Words.8d9ac787-8e37-495e-8d66-5a7693969639.004.png)

disclaimer • S**"O**u**I**ls**n**i**B**ed**lM**e**y**a**"**sn**a**iadn**n**r s**d**ethhf**B**oios**u**urp**s**lId**i**rB**n**eMn**e**so**s**e**s**tannb**P**tade**a**t**r**Bis**t**oh**n**una**e**srim**r**ne**I**eda**n**sr**t**wsk**e**ePi**r**td**n**ah **a**ract**l**snl**U**iee**s**rn**e**t** s  • icPcmoaropauntplducybirtlihatietsrieeti sn lteherwaesfyhiee wrcdaeh inclltIBebeesMd aaiond/n vpeatihiloraarsblteesi.n all and legal  Rpreofeducrencts, eprs ion gtrhiams prs, eosresnteravtiicoen s tdoo I BnoMt  

or anyone else outside of IBM or the 

Business Partners’ company.

- © IBM Corporation 2023.  presentation may change at any time at **All Rights Reserved.** IBM’s sole discretion based on market opportunities or other factors and are 
- The information contained in this  not intended to be a commitment to publication is provided for informational  future product or feature availability in purposes only. While efforts were made  any way. Nothing contained in these 

to verify the completeness and accuracy  materials is intended to, nor shall have IBM and Business Partner  of the information contained in this  the effect of, stating or implying that 

Internal Use Only pwuabrrliacnattyioonf, aitniys  kpirnodv, ideexpdrAeSssI So rwiimthpoliuetd.  any activities undertaken by you will 

In addition, this information is based on  result in any specific sales, revenue IBM’s current product plans and strategy,  growth, or other results. 

which are subject to change by IBM without 

notice. IBM shall not be responsible for  • All client examples described are 

any damages arising out of the use of, or  presented as illustrations of how those otherwise related to, this publication or  clients have used IBM products and the any other materials. Nothing contained in  results, they 

this publication is intended to, nor shall 

may have achieved. Actual 

have the effect of, creating any warranties 

or representations from IBM or its suppliers  environmental costs and performance or licensors, or altering the terms and  characteristics 

conditions of the applicable license  may vary by client.

agreement governing the use of 

IBM software.

watsonx.ai InstructLab FAQs (pg. 1)

**What is InstructLab?** 

InstructLab is a novel way to facilitate Large Language model development through collaboration among the open-source community. Check out th[is link for](https://w3.ibm.com/w3publisher/ai-for-business/instructlab) more details.

**What aspects of InstructLab have been open-sourced?** 

InstructLab consists of a Command Line Interface(cli) and backend for synthetic data generation and model training. Only the front end cli is being open-sourced. For more details refer to this link (to be updated with IL blog)

**Are there any LLMs that were open sourced too?**

Yes! granite-7b-lab that is continually trained with the InstructLab is also open-sourced. You can check out the model on HuggingFace (link to be updated)

**How different is InstructLab from Tuning Studio in watsonx.ai?** 

InstructLab employs a different way of enhancing the LLM by the concept of reusable skills and knowledge and later pretraining the model with them. Tuning Studio employs the concept of prompt tuning to enhance the model s performance. While both these techniques aim at enhancing LLMs  performance, they employ different methods to achieve it.

**What does this mean for watsonx.ai? Are there any plans of bringing in InstructLab into watsonx.ai?**

- Watsonx.ai will ensure a continuous delivery of the most performant version of Granite models.
- Granite-13b-V2.1 chat (InstructLAB-tuned model) has been already available on the platform since Feb 15.
- granite-20b-multilingual is now refreshed with an enhanced InstructLAB version of the model that delivers higher performance.
- granite-7b-lab which is a new open-source language model for English is now available on watsonx.ai SaaS, on-prem coming soon.
- In addition to Granite models, watsonx.ai has provided Merlinite, a LAB-tuned version of Mistral 7B SaaS, coming to on-premises soon.
- For each InstructLab-tuned model, watsonx.ai offers an interactive taxonomy exploration and an evaluation experience to understand the knowledge/skills
- data and taxonomy behind a InstructLab model and the performance improvements achieved.

watsonx.ai InstructLab FAQs (pg. 2)

**What should I say if my customer asks about InstructLab?** 

Today s LLMs are not truly community driven. There are 30K+ Llama and Mistral forks on HuggingFace alone. There is no clear path to contributing and enhancing an existing Language Model. InstructLab offers a novel method for collaborative customization/tuning. Watsonx.ai already supports InstructLab trained models on its platform (granite-7b-lab, granite-20b-multilingual, merlinite-7b, granite-13b-chat-v2(2.1)) with more in the works. A Taxonomy explorer interface is now available in watsonx.ai to view the taxonomy tree that was used to train the model. InstructLab as a tuning method will be offered in Tuning Studio. Today we have Evaluation UI available, with advanced features for skills creation/management and Synthetic Data Generation. Please bookmark watsonx.ai roadmap (link) and stay tuned for more information.

**Who should I contact if I need more information on InstructLab and watsonx.ai collaboration?**

Please feel free to post your question on the [#watsonx-ai-](https://ibm.enterprise.slack.com/archives/C05FWDB9RSA)

[feedback ](https://ibm.enterprise.slack.com/archives/C05FWDB9RSA)Slack channel.

watsonx.ai InstructLab FAQs (pg. 3)

**Ethical AI Use**

Licensee agrees not to, and not to direct or allow third parties, use the IBM developed foundation models, or BYOMs: (i) for mass surveillance, racial profiling, or any use that violates or encourages the violation of basic human rights or other applicable laws and regulations; (ii) to distribute false, misleading, disparaging or obscene information or content; (iii) to provide fully automated decision making in connection use cases involving critical processes or the risk of loss of life, property or impact on an individual’s legal rights; (iv) in a manner that impersonates another for deceptive purposes or conceals the fact a user is interacting with AI; or (v) to distribute or intentionally generate malware or other harmful code.
