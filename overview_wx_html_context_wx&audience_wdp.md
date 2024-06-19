﻿IBMÂ watsonxIBMÂ watsonx Log In Sign Up Branch Pull0 Pull0 Commit0 Commit0 Push0 Push0 Checkout branch Checkout branch Merge conflict Merge conflict Commit history Commit history Git preferences Git preferences Pull and push Pull and push Pull only Pull only Import export Import export Export project Export project Import project Import project Migrate NewAdd Add NewAdd Add Analytics project Analytics project Data Transform project Data Transform project Launch IDE JupyterLab JupyterLab RStudio RStudio Project terminal Project terminal Add to projectAdd Add Add to projectAdd Add Connected assets Connected assets Notebook Notebook Connection Connection Data asset Data asset Scheduled job Scheduled job Model Model FunctionBETA FunctionBETA Synthesized neural networkBETA Synthesized neural networkBETA ExperimentBETA ExperimentBETA Streams flowBETA Streams flowBETA Modeler flow Modeler flow Dashboard Dashboard Data Refinery flow Data Refinery flow Environment Environment Visual recognition model Visual recognition model Natural language classifier model Natural language classifier model Application Application Fork Project Fork Project Export Export Download Download Confirm Do you want to log out? Overview Overview Services and integrations Services and integrations Getting started Getting started AI risk atlas AI risk atlas Projects Projects Preparing data Preparing data Developing generative AI solutions Developing generative AI solutions Analyzing data and working with models Analyzing data and working with models Deploying models and other assets Deploying models and other assets Governing AI assets Governing AI assets Troubleshooting Troubleshooting Administration Administration Glossary Glossary Overview of IBM watsonx as a Service Overview of IBM watsonx as a Service IBM watsonx as a Service is a secure and collaborative environment where you can access your organization's trusted data, automate AI processes, and deliver AI in your applications. The IBM watsonx.ai component provides a studio of integrated tools for working with generative AI capabilities that are powered by foundation models and for building machine learning models. The IBM watsonx.governance component provides end-to-end monitoring for machine learning and generative AI models to accelerate responsible, transparent, and explainable AI workflows. AI engineers, data scientists, and AI risk and compliance officers can accomplish the following goals with watsonx.ai and watsonx.governance: Build machine learning models Build models by using open source frameworks and code-based, automated, or visual data science tools. Develop with foundation models Generate prompts to generate, classify, summarize, or extract content from your input text. Choose from IBM models or open source models from Hugging Face. Tune foundation models to customize your prompt output. Manage the AI lifecycle Manage and automate the full AI model lifecycle with all the integrated tools and runtimes to train, validate, and deploy AI models. Govern AI Track the detailed history of AI models and evaluate model output to help ensure compliance. Data engineers can collect, store, query, and analyze enterprise data in a lakehouse architecture with IBM watsonx.data. See IBM watsonx.data documentation. The following graphic shows the capabilities of the watsonx.ai and watsonx.governance components on top of the common core functionality that provides an integrated user experience. The watsonx.data experience is separate and not shown in the graphic. Watsonx.ai Watsonx.ai includes tools for working with data and models, deployed foundation models for generative AI, and the hardware and software resources for computing and inferencing. Watch this short video that introduces watsonx.ai. Tools for preparing data and working with models Your watsonx.ai tools are in collaborative workspaces called projects. You can use watsonx.ai tools to prepare data and work with models in the following ways: Prepare data: Refine and visualize your data files or data tables in remote data sources or generate synthetic tabular data. Build machine learning models: Automatically generate model candidates, create machine learning model training flows, or write model training code in Python or R. Work with foundation models: Experiment with generative AI prompts, tune foundation models for your use case, or write generative AI solution code in Python. Automate model lifecycles: Create repeatable and scheduled flows that automate notebook, Data Refinery, and machine learning pipelines. For a list of tools, their levels of automation, and whether you can use them to prepare data or work with models, see Analyzing data and working with models. For generative AI tools, see Developing generative AI solutions. Deployed foundation models IBM watsonx.ai has a range of deployed large language models for generative AI. The deployed foundation models include open source models from Hugging Face and IBM foundation models. You can select the appropriate foundation model for your inferencing use case. You can customize foundation model behavior by tuning a foundation model. For a list of supported foundation models that are deployed in watsonx.ai, see Supported foundation models. Usage resources for computing and inference Depending on your service plans, you might have a set amount of usage resources per month or you might be billed for the resources that you consume. When you run tools with watsonx.ai, you consume the following types of resources: Compute usage When you run jobs, notebooks, experiments that train or tune models, or deployments, your compute resource usage is calculated based on the rate for the runtime environment and its active duration. Compute resources include the appropriate hardware and software that are specific for the workload. Compute usage is measured in capacity unit hours. See Choosing compute resources for running tools in projects. Inferencing usage When you run inferencing against foundation models, your inferencing usage is calculated as the sum of the tokens in the prompt input and output text multiplied by the rate for the foundation model. Tokens are basic units of text. Inferencing is measured in resource units. See Resource unit metering. Watsonx.governance Watsonx.governance includes tools for governing models and the usage resources for evaluating and explaining models. Watch this short video that introduces watsonx.governance. Tools for governing models You can use watsonx.governance tools to govern models in the following ways: Monitor and evaluate models: You can monitor model output and explain model predictions. Your watsonx.governance model monitoring and evaluation tools are in projects and deployment spaces. Track and document AI use cases: You can view model lifecycle status, general model and deployment details, training information and metrics, and deployment metrics. Your watsonx.governance model tracking tools in AI use cases. Manage governance activity from the Governance Console Optionally integrate with the watsonx Governance Console from IBM OpenPages. Sync data from factsheets with the Governance Console, and extend governance capabilities with workflows and other compliance tools. Usage resources for model evaluations and explanations When you run model evaluations and explanations with watsonx.governance, you consume resources. Depending on your service plans, you might have a set amount of usage resources per month or you might be billed for the resources that you consume. Your resource usage is calculated based on the number of model evaluations and explanations. Evaluations and explanations are measured in resource units. Common core functionality Watsonx includes the following core functionality of IBM Cloud Pak for Data as the secure and scalable foundation for your organization to collaborate efficiently: Connectivity Administration Storage Workspaces Resource hub Connectivity You can create connections to remote data sources and import connected data. You can configure connections with personal or shared credentials. For a list of supported connectors, see Connectors. You can share connections with others across the platform in the Platform assets catalog. Administration The following administration features provide security and flexibility: Software and hardware Watsonx is fully managed by IBM on IBM Cloud. Software updates are automatic. Scaling of usage resources and storage is automatic. Security, compliance, and isolation The data security, network security, security standards compliance, and isolation of watsonx are managed by IBM Cloud. Data is encrypted at rest and in motion. You can set up extra security and encryption options. Your work on watsonx, including your data and the models that you create, are private to your account. Your data and models will never be accessible or used by IBM or any other person or organization. Learn more about security and your options: Security and privacy of foundation models Data security Security of watsonx Services provisioning Watsonx.ai on the watsonx platform includes the Watson Studio, Watson Machine Learning, and IBM Cloud Object Storage services. Watsonx.governance on the watsonx platform includes the watsonx.governance service. You can add services, such as data source services, from the watsonx services catalog. See Creating and managing IBM Cloud services. User management You add users and user groups and manage their account roles and permissions with IBM Cloud Identity and Access Management. You assign roles within each collaborative workspace across the platform. See Managing users and access. Storage A IBM Cloud Object Storage service instance is automatically provisioned for you to provide storage for the assets that you create or add to workspaces. Information that is stored in IBM Cloud Object Storage is encrypted and resilient. Each workspace has its own dedicated bucket. See Object storage for workspaces. Workspaces Watsonx is organized as a set of collaborative workspaces where you can work with your team or organization. Each workspace has a set of members with roles that provide permissions to perform actions. Most users work with assets, which are items that are created or added to workspaces by users. Assets can represent data, models, or other types of code or information. Data assets contain metadata that represents data. Assets that you create in tools, such as models, run code to work with data. You can also create assets that contain information about other assets, such as model use cases that contain metadata, history, and reports about models. See Asset types and properties. You can work in these types of workspaces in watsonx: Projects Deployment spaces Platform connections AI use cases You can search for assets across all workspaces that you belong to. Projects Projects are where your data science and model builder teams work with data to create assets, such as, saved prompts, notebooks, models, or pipelines. Your first project, which is known as your sandbox project, is created automatically when you sign up for watsonx.ai. See Your sandbox project. The following image shows what the Overview page of a project might look like. Deployment spaces Deployment spaces are where your ModelOps team deploys models and other deployable assets to production and then tests and manages deployments in production. After you build models and deployable assets in projects, you promote them to deployment spaces. See Deployment spaces. The following image shows what the Overview page of a deployment space might look like. Platform connections Platform connections is a view of the Platform assets catalog that lists connection assets. You can access platform connections in any project or deployment space. The following image shows what the Connections page of the Platform connections might look like. AI use cases AI use cases is a view of the Platform assets catalog that lists model use cases. Use cases track the details for AI assets in factsheets. The following image shows what the AI use cases page might look like. Resource hub Watsonx includes an integrated collection of samples that provides deployed foundation models, data assets, prompts, notebooks, and sample projects. Sample notebooks provide examples of data science and machine learning code. Sample projects contain sets of data, models, other assets, and detailed instructions on how to solve a particular business problem. The following image shows what Resource hub looks like. Watch this video to see a tour of the Resource hub. This video provides a visual method to learn the concepts and tasks in this documentation. Learn more Use cases Asset types and properties AI risk atlas Comparison of IBM watsonx as a Service and Cloud Pak for Data as a Service Feature differences between watsonx deployments Foundation models IBM watsonx.data documentation Overview of IBM watsonx as a Service IBM watsonx as a Service is a secure and collaborative environment where you can access your organization's trusted data, automate AI processes, and deliver AI in your applications. The IBM watsonx.ai component provides a studio of integrated tools for working with generative AI capabilities that are powered by foundation models and for building machine learning models. The IBM watsonx.governance component provides end-to-end monitoring for machine learning and generative AI models to accelerate responsible, transparent, and explainable AI workflows. AI engineers, data scientists, and AI risk and compliance officers can accomplish the following goals with watsonx.ai and watsonx.governance: Build machine learning models Build models by using open source frameworks and code-based, automated, or visual data science tools. Build machine learning models Build models by using open source frameworks and code-based, automated, or visual data science tools. Develop with foundation models Generate prompts to generate, classify, summarize, or extract content from your input text. Choose from IBM models or open source models from Hugging Face. Tune foundation models to customize your prompt output. Develop with foundation models Generate prompts to generate, classify, summarize, or extract content from your input text. Choose from IBM models or open source models from Hugging Face. Tune foundation models to customize your prompt output. Manage the AI lifecycle Manage and automate the full AI model lifecycle with all the integrated tools and runtimes to train, validate, and deploy AI models. Manage the AI lifecycle Manage and automate the full AI model lifecycle with all the integrated tools and runtimes to train, validate, and deploy AI models. Govern AI Track the detailed history of AI models and evaluate model output to help ensure compliance. Govern AI Track the detailed history of AI models and evaluate model output to help ensure compliance. Data engineers can collect, store, query, and analyze enterprise data in a lakehouse architecture with IBM watsonx.data. See IBM watsonx.data documentation. IBM watsonx.data documentation The following graphic shows the capabilities of the watsonx.ai and watsonx.governance components on top of the common core functionality that provides an integrated user experience. The watsonx.data experience is separate and not shown in the graphic. Watsonx.ai Watsonx.ai includes tools for working with data and models, deployed foundation models for generative AI, and the hardware and software resources for computing and inferencing. Watch this short video that introduces watsonx.ai. Tools for preparing data and working with models Your watsonx.ai tools are in collaborative workspaces called projects. You can use watsonx.ai tools to prepare data and work with models in the following ways: Prepare data: Refine and visualize your data files or data tables in remote data sources or generate synthetic tabular data. Build machine learning models: Automatically generate model candidates, create machine learning model training flows, or write model training code in Python or R. Work with foundation models: Experiment with generative AI prompts, tune foundation models for your use case, or write generative AI solution code in Python. Automate model lifecycles: Create repeatable and scheduled flows that automate notebook, Data Refinery, and machine learning pipelines. For a list of tools, their levels of automation, and whether you can use them to prepare data or work with models, see Analyzing data and working with models. For generative AI tools, see Developing generative AI solutions. Analyzing data and working with models Developing generative AI solutions Deployed foundation models IBM watsonx.ai has a range of deployed large language models for generative AI. The deployed foundation models include open source models from Hugging Face and IBM foundation models. You can select the appropriate foundation model for your inferencing use case. You can customize foundation model behavior by tuning a foundation model. For a list of supported foundation models that are deployed in watsonx.ai, see Supported foundation models. Supported foundation models Usage resources for computing and inference Depending on your service plans, you might have a set amount of usage resources per month or you might be billed for the resources that you consume. When you run tools with watsonx.ai, you consume the following types of resources: Choosing compute resources for running tools in projects Resource unit metering Watsonx.governance Watsonx.governance includes tools for governing models and the usage resources for evaluating and explaining models. Watch this short video that introduces watsonx.governance. Tools for governing models You can use watsonx.governance tools to govern models in the following ways: Monitor and evaluate models: You can monitor model output and explain model predictions. Your watsonx.governance model monitoring and evaluation tools are in projects and deployment spaces. Monitor and evaluate