﻿IBM Cloud Docs Skip to contentIBM CloudCatalogCatalogCost EstimatorCost EstimatorHelpHelpDocsLog inSign upError Skip to content IBM Cloud IBM Cloud CatalogCatalog CatalogCatalog Cost EstimatorCost Estimator Cost EstimatorCost Estimator HelpHelpDocs HelpHelp Docs Docs Docs Log in Log in Sign up Sign up Error Provisioning a Presto engine Provisioning a Presto engine The engine runs SQL queries on your data source and fetches the queried data. watsonx.data allows provisioning a Presto engine. The following versions of Presto engine are supported as per specified watsonx.data versions: watsonx.data v1.0.0, v1.0.1 and v1.0.2: Presto version 0.279 watsonx.data v1.0.3, v1.1.1 and v1.1.3: Presto version 0.282 watsonx.data v1.1.4: Presto version 0.285.1 To provision a Presto engine, complete the following steps. Log in to watsonx.data console. From the navigation menu, select Infrastructure manager. To provision an engine, click Add component and select Add engine. In the Add engine window, select Presto(version) from the Type drop-down list. Configure the following engine details. Table 1. Provision engine Field Description Display name Enter your compute engine name. Configuration mode Select Standard for predefined engine sizes or Custom for customized engine configuration. Size Select the engine size. For all sizes, coordinator and worker nodes are storage-optimized. The field appears when you select the Configuration mode as Standard. Coordinator nodes (max.1) Select the size for the coordinator node. The field appears when you select the Configuration mode as Custom. Worker nodes (max.18) Select the size required for worker node. The field appears when you select the Configuration mode as Custom. Associated Catalogs (optional) Associate the available catalogs with the engine if necessary. Click Provision(0+RUs/hour) to provision the Presto engine. Provisioning a Presto engine The engine runs SQL queries on your data source and fetches the queried data. watsonx.data allows provisioning a Presto engine. The following versions of Presto engine are supported as per specified watsonx.data versions: watsonx.data v1.0.0, v1.0.1 and v1.0.2: Presto version 0.279 watsonx.data v1.0.0, v1.0.1 and v1.0.2: Presto version 0.279 Presto version 0.279 watsonx.data v1.0.3, v1.1.1 and v1.1.3: Presto version 0.282 watsonx.data v1.0.3, v1.1.1 and v1.1.3: Presto version 0.282 Presto version 0.282 watsonx.data v1.1.4: Presto version 0.285.1 watsonx.data v1.1.4: Presto version 0.285.1 Presto version 0.285.1 To provision a Presto engine, complete the following steps. Log in to watsonx.data console. Log in to watsonx.data console. From the navigation menu, select Infrastructure manager. From the navigation menu, select Infrastructure manager. To provision an engine, click Add component and select Add engine. To provision an engine, click Add component and select Add engine. In the Add engine window, select Presto(version) from the Type drop-down list. In the Add engine window, select Presto(version) from the Type drop-down list. Configure the following engine details. Table 1. Provision engine Field Description Display name Enter your compute engine name. Configuration mode Select Standard for predefined engine sizes or Custom for customized engine configuration. Size Select the engine size. For all sizes, coordinator and worker nodes are storage- optimized. The field appears when you select the Configuration mode as Standard. Coordinator nodes (max.1) Select the size for the coordinator node. The field appears when you select the Configuration mode as Custom. Worker nodes (max.18) Select the size required for worker node. The field appears when you select the Configuration mode as Custom. Associated Catalogs (optional) Associate the available catalogs with the engine if necessary. Configure the following engine details. Display name Enter your compute engine name. Configuration mode Select Standard for predefined engine sizes or Custom for customized engine configuration. Size Select the engine size. For all sizes, coordinator and worker nodes are storage-optimized. The field appears when you select the Configuration mode as Standard. Coordinator nodes (max.1) Select the size for the coordinator node. The field appears when you select the Configuration mode as Custom. Worker nodes (max.18) Select the size required for worker node. The field appears when you select the Configuration mode as Custom. Associated Catalogs (optional) Associate the available catalogs with the engine if necessary. Click Provision(0+RUs/hour) to provision the Presto engine. Click Provision(0+RUs/hour) to provision the Presto engine.