﻿Generative AI thatâ€™s tailored for your business needs with watsonx.ai AI for the Enterprise Dinesh Nirmal According to a recent IBV study, 64% of surveyed CEOs face pressure to accelerate adoption of generative AI, and 60% lack a consistent, enterprise-wide method for implementing it. An AI and data platform, such as watsonx, can help empower businesses to leverage foundation models and accelerate the pace of generative AI adoption across their organization. The newly launched features and capabilities of watsonx.ai, a capability within watsonx, include new general-purpose and code-generation foundation models, an increased variety of open-source model options, and additional data options and tuning capabilities that can broaden the potential business impact of generative AI. These enhancements have been guided by IBMâ€™s fundamental strategic considerations that AI should be open, trusted, targeted and empowering. Learn more about watsonx.ai, our enterprise- focused studio for AI builders. Business-targeted, IBM-developed foundation models built from sound data Business leaders charged with adopting generative AI need model flexibility and choice. They also need secured access to business-relevant models that can help accelerate time to value and insights. Recognizing that one size doesnâ€™t fit all, IBMâ€™s watsonx.ai studio provides a family of language and code foundation models of different sizes and architectures to help clients deliver performance, speed, and efficiency. â€œIn an environment where the integration with our systems and seamless interconnection with various software are paramount, watsonx.ai emerges as a compelling solution,â€ says Atsushi Hasegawa, Chief Engineer, Honda R&D. â€œIts inherent flexibility and agile deployment capabilities, coupled with a robust commitment to information security, accentuates its appeal.â€ The initial release of watsonx.ai included the Slate family of encoder-only models useful for enterprise NLP tasks. Weâ€™re happy to now introduce the first iteration of our IBM-developed generative foundation models, Granite. The Granite model series is built on a decoder-only architecture and is suited to generative tasks such as summarization, content generation, retrieval- augmented generation, classification, and extracting insights. All Granite foundation models have been trained on enterprise-focused datasets curated by IBM. Â To provide even deeper domain expertise, the Granite family of models was trained on enterprise-relevant datasets from five domains: internet, academic, code, legal and finance, all scrutinized to root out objectionable content, and benchmarked against internal and external models. This process is designed to help mitigate risks so that model outputs can be deployed responsibly with the assistance of watsonx.data and watsonx.governance (coming soon). Based on initial IBM Research evaluations and testing, across 11 different financial tasks, the results show that by training Granite-13B models with high-quality finance data, they are some of the top performing models on finance tasks, and have the potential to achieve either similar or even better performance than much larger models. Financial tasks evaluated includes: providing sentiment scores for stock and earnings call transcripts, classifying news headlines, extracting credit risk assessments, summarizing financial long- form text and answering financial or insurance-related questions. Building transparency into IBM-developed AI models To date, many available AI models lack information about data provenance, testing and safety or performance parameters.Â For many businesses and organizations, this can introduce uncertainties that slow adoption of generative AI, particularly in highly regulated industries. Today, IBM is sharing the following data sources used in the training of the Granite models (learn more about how these models are trained and data sources used): Common Crawl Webhose GitHub Clean Arxiv USPTO Pub Med Central SEC Filings Free Law Wikimedia Stack Exchange DeepMind Mathematics Project Gutenberg (PG-19) OpenWeb Text HackerNews IBMâ€™s approach to AI development is guided by core principles grounded in commitments to trust and transparency. As a testament to the rigor IBM puts into the development and testing of its foundation models,Â IBM will

indemnifyÂ clients against third party IP claims against IBM-developed foundation models. And contrary to some other providers of Large Language Models and consistent with IBMâ€™s standard approach on indemnification, IBM does not require its customers to indemnify IBM for a customerâ€™s use of IBM developed models. Also consistent with IBMâ€™s approach to its indemnification obligation, IBM does not cap its IP indemnification liability for the IBM-developed models. As clients look to use our IBM-developed models to create differentiated AI assets, we encourage clients to further customize IBM models to meet specific downstream tasks. Through prompt engineering and tuning techniques underway, clients can responsibly use their own enterprise data to achieve greater accuracy in the model outputs, to create a competitive edge.Â Helping organizations responsibly use third-party models Considering there are thousands of open-source large language models to work with, itâ€™s difficult to know where to get started and how to choose the right model for the right task. However, choosing the â€œrightâ€ LLM from a collection of thousands of open-source models is not an easy endeavor and requires a careful examination of the tradeoffs between cost and performance. And considering the unpredictability of many LLMs, itâ€™s important to also factor in AI ethics and governance into the model building, training, tuning, testing, and outputs. Knowing that one model wonâ€™t be enough â€“ weâ€™ve created a foundation model library in watsonx.ai for clients and partners to work with. Starting with 5 curated open-source models from Hugging Face, we chose these models based on rigorous technical, licensing and performance reviews, and includes understanding the range of use cases that the models are best for. The latest open-source LLM model we added this month includes Metaâ€™s 70 billion parameter model Llama 2-chat inside the watsonx.ai studio. Llama 2 is useful for chat and code generation. It is pretrained with publicly available online data and fine-tuned using reinforcement learning from human feedback. Useful for enhancing virtual agent and chat applications, Llama 2 is intended for commercial and research scenarios. The StarCoder LLM from BigCode is also now available in watsonx.ai. Trained on permissively licensed data from GitHub, the model can be used as a technical assistant, explaining, and answering general questions about code in natural language. It can also help autocomplete code, modify code and explain code snippets in natural language. Users of third-party models in watsonx.ai can also toggle on an AI guardrails function to help automatically remove offensive language from input prompts and generated output. Reducing model-training risk with synthetic data In the conventional process of anonymizing data, errors can be introduced that severely compromise outputs and predictions. But synthetic data offers organizations the ability to address data gaps and reduce the risk of exposing any individualâ€™s personal data by taking advantage of data created artificially through computer simulation or algorithms. The synthetic data generator service in watsonx.ai will enable organizations to create synthetic tabular data that is pre-labeled and preserves the statistical properties of their original enterprise data. Â This data can then be used to tune AI models more quickly or improve their accuracy by injecting more variety into datasets (shortcutting the long data-collection timeframes required to capture the wide variation in real data). Being able to build and test models with synthetic data can help organizations overcome data gaps and, in turn, improve their speed to market with new AI solutions. Enabling business-focused use cases with prompt tuning The official release of Tuning Studio in watsonx.ai lets business users customize foundation models to their business-specific downstream needs across a variety of use cases including Q&A, content generation, named entity recognition, insight extraction, summarization, and classification. The first release of the Tuning Studio will support prompt tuning. By using advanced prompt tuning within watsonx.ai (based on as few as 100 to 1,000 examples), organizations can customize existing foundation models to their proprietary data. Prompt-tuning allows a company with limited data to tailor a massive model to a narrow task, with the potential to reduce computing and energy use without having to retrain an AI model. Advancing and supporting AI for business The IBM watsonx AI and data platform is built for business, designed to help more individuals in your organization scale and accelerate the impact of AI with your trusted data. As AI technologies advance, the watsonx architecture is designed to smoothly integrate new business-targeted foundation models such as those developed by IBM Research, and to accommodate third-party models such as those provided on the Hugging Face open-source platform, while providing critical governance guardrails with the future release of watsonx.governance. The watsonx platform is just one part of IBMâ€™s generative AI solutions. With IBM Consulting clients can get help tuning and operationalizing models for targeted business use cases with access to the specialized generative AI expertise of more than 1,000 consultants. Test out watsonx.ai with our watsonx trial experience Was this article helpful?YesNo According to a recent IBV study, 64% of surveyed CEOs face pressure to accelerate adoption of generative AI, and 60% lack a consistent, enterprise-wide method for implementing it. recent IBV study An AI and data platform, such as watsonx, can help empower businesses to leverage foundation models and accelerate the pace of generative AI adoption across their organization. The newly launched features and capabilities of watsonx.ai, a capability within watsonx, include new general-purpose and code-generation foundation models, an increased variety of open-source model options, and additional data options and tuning capabilities that can broaden the potential business impact of generative AI. These enhancements have been guided by IBMâ€™s fundamental strategic considerations that AI should be open, trusted, targeted and empowering. open, trusted, targeted and empowering Learn more about watsonx.ai, our enterprise-focused studio for AI builders. Learn more about watsonx.ai, our enterprise-focused studio for AI builders. Business-targeted, IBM-developed foundation models built from sound data Business leaders charged with adopting generative AI need model flexibility and choice. They also need secured access to business-relevant models that can help accelerate time to value and insights. Recognizing that one size doesnâ€™t fit all, IBMâ€™s watsonx.ai studio provides a family of language and code foundation models of different sizes and architectures to help clients deliver performance, speed, and efficiency. â€œIn an environment where the integration with our systems and seamless interconnection with various software are paramount, watsonx.ai emerges as a compelling solution,â€ says Atsushi Hasegawa, Chief Engineer, Honda R&D. â€œIts inherent flexibility and agile deployment capabilities, coupled with a robust commitment to information security, accentuates its appeal.â€ The initial release of watsonx.ai included the Slate family of encoder-only models useful for enterprise NLP tasks. Weâ€™re happy to now introduce the first iteration of our IBM-developed generative foundation models, Granite. The Granite model series is built on a decoder-only architecture and is suited to generative tasks such as summarization, content generation, retrieval-augmented generation, classification, and extracting insights. Granite All Granite foundation models have been trained on enterprise-focused datasets curated by IBM. Â To provide even deeper domain expertise, the Granite family of models was trained on enterprise-relevant datasets from five domains: internet, academic, code, legal and finance, all scrutinized to root out objectionable content, and benchmarked against internal and external models. This process is designed to help mitigate risks so that model outputs can be deployed responsibly with the assistance of watsonx.data and watsonx.governance (coming soon). Based on initial IBM Research evaluations and testing, across 11 different financial tasks, the results show that by training Granite-13B models with high-quality finance data, they are some of the top performing models on finance tasks, and have the potential to achieve either similar or even better performance than much larger models. Financial tasks evaluated includes: providing sentiment scores for stock and earnings call transcripts, classifying news headlines, extracting credit risk assessments, summarizing financial long-form text and answering financial or insurance-related questions. IBM Research evaluations and testing Building transparency into IBM-developed AI models To date, many available AI models lack information about data provenance, testing and safety or performance parameters.Â For many businesses and organizations, this can introduce uncertainties that slow adoption of generative AI, particularly in highly regulated industries. Today, IBM is sharing the following data sources used in the training of the Granite models (learn more about how these models are trained and data sources used): learn more about how these models are trained and data sources used Common Crawl Webhose GitHub Clean Arxiv USPTO Pub Med Central SEC Filings Free Law Wikimedia Stack Exchange DeepMind Mathematics Project Gutenberg (PG-19) OpenWeb Text HackerNews IBMâ€™s approach to AI development is guided by core principles grounded in commitments to trust and transparency. As a testament to the rigor IBM puts into the development and testing of its foundation models,Â IBM will indemnifyÂ clients against third party IP claims against IBM-developed foundation models. And contrary to some other providers of Large Language Models and consistent with IBMâ€™s standard approach on indemnification, IBM does not require its customers to indemnify IBM for a customerâ€™s use of IBM developed models. Also consistent with IBMâ€™s approach to its indemnification obligation, IBM does not cap its IP indemnification liability for the IBM-developed models. core principles IBM will indemnify As clients look to use our IBM-developed models to create differentiated AI assets, we encourage clients to further customize IBM models to meet specific downstream tasks. Through prompt engineering and tuning techniques underway, clients can responsibly use their own enterprise data to achieve greater accuracy in the model outputs, to create a competitive edge.Â  Helping organizations responsibly use third-party models Considering there are thousands of open-source large language models to work with, itâ€™s difficult to know where to get started and how to choose the right model for the right task. However, choosing the â€œrightâ€ LLM from a collection of thousands of open-source models is not an easy endeavor and requires a careful examination of the tradeoffs between cost and performance. And considering the unpredictability of many LLMs, itâ€™s important to also factor in AI ethics and governance into the model building, training, tuning, testing, and outputs. Knowing that one model wonâ€™t be enough â€“ weâ€™ve created a foundation model library in watsonx.ai for clients and partners to work with. Starting with 5 curated open-source models from Hugging Face, we chose these models based on rigorous technical, licensing and performance reviews, and includes understanding the range of use cases that the models are best for. The latest open-source LLM model we added this month includes Metaâ€™s 70 billion parameter model Llama 2-chat inside the watsonx.ai studio. Llama 2 is useful for chat and code generation. It is pretrained with publicly available online data and fine-tuned using reinforcement learning from human feedback. Useful for enhancing virtual agent and chat applications, Llama 2 is intended for commercial and research scenarios. fine-tuned using reinforcement learning The StarCoder LLM from BigCode is also now available in watsonx.ai. Trained on permissively licensed data from GitHub, the model can be used as a technical assistant, explaining, and answering general questions about code in natural language. It can also help autocomplete code, modify code and explain code snippets in natural language. StarCoder LLM Users of third-party models in watsonx.ai can also toggle on an AI guardrails function to help automatically remove offensive language from input prompts and generated output. Reducing model-training risk with synthetic data In the conventional process of anonymizing data, errors can be introduced that severely compromise outputs and predictions. But synthetic data offers organizations the ability to address data gaps and reduce the risk of exposing any individualâ€™s personal data by taking advantage of data created artificially through computer simulation or algorithms. synthetic data The synthetic data generator service in watsonx.ai will enable organizations to create synthetic tabular data that is pre-labeled and preserves the statistical properties of their original enterprise data. Â This data can then be used to tune AI models more quickly or improve their accuracy by injecting more variety into datasets (shortcutting the long data-collection timeframes required to capture the wide variation in real data). Being able to build and test models with synthetic data can help organizations overcome data gaps and, in turn, improve their speed to market with new AI solutions. Enabling business-focused use cases with prompt tuning The official release of Tuning Studio in watsonx.ai lets business users customize foundation models to their business-specific downstream needs across a variety of use cases