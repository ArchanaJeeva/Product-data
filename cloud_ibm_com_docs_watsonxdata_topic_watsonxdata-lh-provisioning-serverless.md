﻿IBM Cloud Docs Skip to contentIBM CloudCatalogCatalogCost EstimatorCost EstimatorHelpHelpDocsLog inSign upError Skip to content IBM Cloud IBM Cloud CatalogCatalog CatalogCatalog Cost EstimatorCost Estimator Cost EstimatorCost Estimator HelpHelpDocs HelpHelp Docs Docs Docs Log in Log in Sign up Sign up Error Provisioning Analytics Engine Provisioning Analytics Engine For watsonx.data, it is recommended to use IBM Analytics Engine Spark to achieve below use-cases: Ingesting large volumes of data into watsonx.data tables. You can also cleanse and transform data before ingestion. Table maintenance operation to enhance watsonx.data performance of the table Complex analytics workload which are difficult to represent as queries. You can create an IBM Analytics Engine instance: Using the IBM CloudÂ® console Using the IBM CloudÂ® command-line interface Using the Resource controller REST API You must have access to either the IBM CloudÂ® us-south (Dallas) or the eu-de (Frankfurt) region. When you add a region for provisioning an Analytics Engine instance, choose one that is closer to the region where you have provisioned watsonx.data to avoid data latency issues. Creating a service instance from the IBM CloudÂ® console You can create an instance by using the IBM CloudÂ® console. To create an IBM Analytics Engine instance: Log in to the IBM CloudÂ® console. Click Services and select the category Analytics. Search for Analytics Engine and then click the tile to open the service instance creation page. Choose the location that is closer to the region where you have provisioned watsonx.data for deploying the service instance. Currently, us-south and eu-de are the only supported regions. Select a plan. Currently, Standard Serverless for Apache Spark is the only supported serverless plan. Configure the instance by entering a name of your choice, selecting a resource group and adding tags. Select latest runtime version available (for example 3.3). Select the IBM Cloud Object Storage instance from your account that you want to use as the Analytics Engine instance home to store instance- related data. Click Create to provision the service instance in the background. The newly created service is listed in your IBM CloudÂ® resource list under Services. Creating a service instance by using the IBM CloudÂ® command-line interface To create a service instance by using the IBM CloudÂ® command-line interface: Download and configure the IBM CloudÂ® CLI. Follow the instructions in Getting started with the IBM CloudÂ® CLI. Set the API endpoint for your region and log in: ibmcloud api https://DOMAIN\_NAME ibmcloud login Parameter value: DOMAIN\_NAME: The API endpoint for your region. For example, cloud.ibm.com Get the list of the resource groups for your account and select one of the returned resource groups as the target resource group in which to create the IBM Analytics Engine serverless instance: ibmcloud resource groups ibmcloud target -g Parameter value: RESOURCE\_GROUP\_NAME: Provide the same name as you specified while provisioning watsonx.data for efficient organizing. Create a service instance: ibmcloud resource service-instance-create ibmanalyticsengine -p @ Parameter value: SERVICE\_INSTANCE\_NAME: Specify a name for the instance. PLAN\_NAME: Specify the plan name as plan\_name8afde05e-5fd8- 4359-a597-946d8432dd45. REGION: Specify the region where you like to provision the instance. Note that currently, standard-serverless-spark is the only supported serverless plan and us-south and eu-de the only supported regions. Choose one that is closer to the region where you have provisioned watsonx.data. PATH\_to JSON file: Include the path to the JSON file that contains the provisioning parameters. For example, for the Dallas region: ibmcloud resource service-instance-create MyServiceInstance ibmanalyticsengine standard-serverless-spark us-south -p @provision.json You can give the service instance any name you choose. Note that currently, standard-serverless-spark is the only supported serverless plan and us-south and eu-de the only supported regions. The provision.json file contains the provisioning parameters for the instance that you want to create. The endpoint to your IBM CloudÂ® Object Storage instance in the payload JSON file must be the direct endpoint. Direct endpoints provide better performance than public endpoints and do not incur charges for any outgoing or incoming bandwidth. Following is a sample provision.json file. { "default\_runtime": { "spark\_version": "3.3" }, "instance\_home": { "region": "us-south", "endpoint": "https://s3.direct.us- south.cloud-object-storage.appdomain.cloud", "hmac\_access\_key": " as ... OK Service instance MyServiceInstance was created. Name: MyServiceInstance ID: crn:v1:staging:public:ibmanalyticsengine:us-south:a/d628eae2cc7e4373bb0c9d2229f2ece5:1e32e\*\*\*-afd9-483a-b1\*\*- 724ba5cf4\*\*\*:: GUID: 1e32e\*\*\*-afd9-483a-b1\*\*-724ba5cf4\*\*\* Location: us-south State: provisioning Type: service\_instance Sub Type: Service Endpoints: public Allow Cleanup: false Locked: false Created at: 2021-11-29T07:20:40Z Updated at: 2021-11-29T07:20:42Z Last Operation: Status create in progress Message Started create instance operation The sample response to the create instance command is: Creating service instance MyServiceInstance in resource group Default of account as ... OK Service instance MyServiceInstance was created. Name: MyServiceInstance ID: crn:v1:staging:public:ibmanalyticsengine:us-south:a/d628eae2cc7e4373bb0c9d2229f2ece5:1e32e\*\*\*-afd9-483a-b1\*\*- 724ba5cf4\*\*\*:: GUID: 1e32e\*\*\*-afd9-483a-b1\*\*-724ba5cf4\*\*\* Location: us-south State: provisioning Type: service\_instance Sub Type: Service Endpoints: public Allow Cleanup: false Locked: false Created at: 2021-11-29T07:20:40Z Updated at: 2021-11-29T07:20:42Z Last Operation: Status create in progress Message Started create instance operation Make a note of the instance ID from the output. You will need the instance ID when you call instance management or Spark application management APIs. See Spark application REST API. Track instance readiness. Creating a service instance by using the Resource controller REST API An IBM Analytics Engine serverless instance must reside in an IBM CloudÂ® resource group. As a first step toward creating an IBM Analytics Engine serverless instance through the Resource controller REST API, you must have the resource group ID and serverless plan ID close at hand. To create a service instance by using the Resource controller REST API: Get the resource group ID by logging in to the IBM CloudÂ® CLI and running the following command: ibmcloud resource groups Sample result: Retrieving all resource groups under account OK Name ID Default Group State Default XXXXX true ACTIVE Use the following resource plan ID for the Standard Serverless for Apache Spark plan: 8afde05e-5fd8-4359-a597-946d8432dd45 Get the IAM token. For instructions, see steps. Create an instance by using the Resource controller REST API: curl -X POST https://resource- controller.cloud.ibm.com/v2/resource\_instances/ --header "Authorization: Bearer $token" -H 'Content-Type: application/json' -d @provision.json The provision.json file contains the provisioning parameters for the instance that you want to create. See Architecture and concepts in serverless instances for a description of the provisioning parameters in the payload. Following is a sample of the provision.json file. { "name": "your-service- instance-name", "resource\_plan\_id": "8afde05e-5fd8-4359-a597-946d8432dd45", "resource\_group": "resource-group-id", "target": "us-south", "parameters": { "default\_runtime": { "spark\_version": "3.3" }, "instance\_home": { "region": "us-south", "endpoint": "s3.direct.us-south.cloud-object- storage.appdomain.cloud", "hmac\_access\_key": "your-access-key", "hmac\_secret\_key": "your-secret-key" } } } Track instance readiness. For more information on the Resource controller REST API for creating an instance, see Create (provision) a new resource instance. Tracking instance readiness To run applications on a newly created serverless instance, the instance must be in active state. To track instance readiness: Enter the following command:curl -X GET https://api.us-south.ae.cloud.ibm.com/v3/analytics\_engines/{instance\_id} -H "Authorization: Bearer $token" Sample response:{ "id": "dc0e\*\*\*\*-eab2-4t9e-9441-56620949\*\*\*\*", "state": "created", "state\_change\_time": "2021-04-21T04:24:01Z", "default\_runtime": { "spark\_version": "3.3", "instance\_home": { "provider": "ibm-cos", "type": "objectstore", "region": "us-south", "endpoint": "https://s3.direct.us-south.cloud-object-storage.appdomain.cloud", "bucket": "ae-bucket-do-not-delete-dc0e\*\*\*\*-eab2-4t\*\*-9441- 566209499546", "hmac\_access\_key": "eH\*\*\*\*g=", "hmac\_secret\_key": "4d\*\*\*\*\*\*\*\*76" }, "default\_config": { "spark.driver.memory": "4g", "spark.driver.cores": 1 } } } Check the value of the state attribute. It must be active before you can start running applications in the instance. Learn more When provisioning serverless instances, follow the recommended Best practices. Provisioning Analytics Engine For watsonx.data, it is recommended to use IBM Analytics Engine Spark to achieve below use-cases: Ingesting large volumes of data into watsonx.data tables. You can also cleanse and transform data before ingestion. Table maintenance operation to enhance watsonx.data performance of the table Complex analytics workload which are difficult to represent as queries. You can create an IBM Analytics Engine instance: Using the IBM CloudÂ® console Using the IBM CloudÂ® console Using the IBM CloudÂ® command-line interface Using the IBM CloudÂ® command-line interface Using the Resource controller REST API Using the Resource controller REST API You must have access to either the IBM CloudÂ® us-south (Dallas) or the eu-de (Frankfurt) region. When you add a region for provisioning an Analytics Engine instance, choose one that is closer to the region where you have provisioned watsonx.data to avoid data latency issues. Creating a service instance from the IBM CloudÂ® console You can create an instance by using the IBM CloudÂ® console. To create an IBM Analytics Engine instance: Log in to the IBM CloudÂ® console. Log in to the IBM CloudÂ® console. IBM CloudÂ® console Click Services and select the category Analytics. Click Services and select the category Analytics. Search for Analytics Engine and then click the tile to open the service instance creation page. Search for Analytics Engine and then click the tile to open the service instance creation page. Choose the location that is closer to the region where you have provisioned watsonx.data for deploying the service instance. Currently, us-south and eu-de are the only supported regions. Choose the location that is closer to the region where you have provisioned watsonx.data for deploying the service instance. Currently, us-south and eu-de are the only supported regions. Select a plan. Currently, Standard Serverless for Apache Spark is the only supported serverless plan. Select a plan. Currently, Standard Serverless for Apache Spark is the only supported serverless plan. Configure the instance by entering a name of your choice, selecting a resource group and adding tags. Configure the instance by entering a name of your choice, selecting a resource group and adding tags. Select latest runtime version available (for example 3.3). Select latest runtime version available (for example 3.3). Select the IBM Cloud Object Storage instance from your account that you want to use as the Analytics Engine instance home to store instance-related data. Select the IBM Cloud Object Storage instance from your account that you want to use as the Analytics Engine instance home to store instance-related data. Click Create to provision the service instance in the background. The newly created service is listed in your IBM CloudÂ® resource list under Services. Click Create to provision the service instance in the background. The newly created service is listed in your IBM CloudÂ® resource list under Services. IBM CloudÂ® resource list Creating a service instance by using the IBM CloudÂ® command-line interface To create a service instance by using the IBM CloudÂ® command-line interface: Download and configure the IBM CloudÂ® CLI. Follow the instructions in Getting started with the IBM CloudÂ® CLI. Download and configure the IBM CloudÂ® CLI. Follow the instructions in Getting started with the IBM CloudÂ® CLI. Getting started with the IBM CloudÂ® CLI Set the API endpoint for your region and log in: ibmcloud api https://DOMAIN\_NAME ibmcloud login Parameter value: DOMAIN\_NAME: The API endpoint for your region. For example, cloud.ibm.com Set the API endpoint for your region and log in: Parameter value: DOMAIN\_NAME: The API endpoint for your region. For example, cloud.ibm.com Get the list of the resource groups for your account and select one of the returned resource groups as the target resource group in which to create the IBM Analytics Engine serverless instance: ibmcloud resource groups ibmcloud target -g Parameter value: RESOURCE\_GROUP\_NAME: Provide the same name as you specified while provisioning watsonx.data for efficient organizing. Get the list of the resource groups for your account and select one of the returned resource groups as the target resource group in which to create the IBM Analytics Engine serverless instance: Parameter value: RESOURCE\_GROUP\_NAME: Provide the same name as you specified while provisioning watsonx.data for efficient organizing. Create a service instance: ibmcloud resource service-instance-create ibmanalyticsengine -p @ Parameter value: SERVICE\_INSTANCE\_NAME: Specify a name for the instance. PLAN\_NAME: Specify the plan name as plan\_name8afde05e-5fd8-4359-a597-946d8432dd45. REGION: Specify the region where you like to provision the instance. Note that currently, standard-serverless-spark is the only supported serverless plan and us-south and eu- de the only supported regions. Choose one that is closer to the region where you have provisioned watsonx.data. PATH\_to JSON file: Include the path to the JSON file that contains the provisioning parameters. For example, for the Dallas region: ibmcloud resource service-instance-create MyServiceInstance ibmanalyticsengine standard-serverless-spark us-south -p @provision.json You can give the service instance any name you choose. Note that currently, standard-serverless-spark is the only supported serverless plan and us-south and eu-de the only supported regions. The provision.json file contains the provisioning parameters for the instance that you want to create. The endpoint to your IBM CloudÂ® Object Storage instance in the payload JSON file must be the direct endpoint. Direct endpoints provide better performance than public endpoints and do not incur charges for any outgoing or incoming bandwidth. Following is a sample provision.json file. { "default\_runtime": { "spark\_version": "3.3" }, "instance\_home": { "region": "us-south", "endpoint": "https://s3.direct.us-south.cloud-object-storage.appdomain.cloud", "hmac\_access\_key": " as ... OK Service instance MyServiceInstance was created. Name: MyServiceInstance ID: crn:v1:staging:public:ibmanalyticsengine:us- south:a/d628eae2cc7e4373bb0c9d2229f2ece5:1e32e\*\*\*-afd9-483a-b1\*\*-724ba5cf4\*\*\*:: GUID: 1e32e\*\*\*-afd9-483a-b1\*\*-724ba5cf4\*\*\* Location: us-south State: provisioning Type: service\_instance Sub Type: Service Endpoints: public Allow Cleanup: false Locked: false Created at: 2021-11-29T07:20:40Z Updated at: 2021-11-29T07:20:42Z Last Operation: Status create in progress Message Started create instance operation The sample response to the create instance command is: Creating service instance MyServiceInstance in resource group Default of account as ... OK Service instance MyServiceInstance was created. Name: MyServiceInstance ID: crn:v1:staging:public:ibmanalyticsengine:us- south:a/d628eae2cc7e4373bb0c9d2229f2ece5:1e32e\*\*\*-afd9-483a-b1\*\*-724ba5cf4\*\*\*:: GUID: 1e32e\*\*\*-afd9-483a-b1\*\*-724ba5cf4\*\*\* Location: us-south State: provisioning Type: service\_instance Sub Type: Service Endpoints: public Allow Cleanup: false Locked: false Created at: 2021-11-29T07:20:40Z Updated at: 2021-11-29T07:20:42Z Last Operation: Status create in progress Message Started create instance operation Make a note of the instance ID from the output. You will need the instance ID when you call instance management or Spark application management APIs. See Spark application REST API. Create a service instance: Parameter value: SERVICE\_INSTANCE\_NAME: Specify a name for the instance. PLAN\_NAME: Specify the plan name as plan\_name8afde05e-5fd8-4359-a597-946d8432dd45. REGION: Specify the region where you like to provision the instance. Note that currently, standard-serverless-spark is the only supported serverless plan and us-south and eu-de the only supported regions. Choose one that is closer to the region where you have provisioned watsonx.data. PATH\_to JSON file: Include the path to the JSON file that contains the provisioning parameters. For example, for the Dallas region: You can give the service instance any name you choose. Note that currently, standard-serverless-spark is the only supported serverless plan and us-south and eu-de the only supported regions. The provision.json file contains the provisioning parameters for the instance that you want to create. The endpoint to your IBM CloudÂ® Object Storage instance in the payload JSON file must be the direct endpoint. Direct endpoints provide better performance than public endpoints and do not incur charges for any outgoing or incoming bandwidth. Following is a sample provision.json file. The IBM CloudÂ® response to the create instance command: The sample response to the create instance command is: Make a note of the instance ID from the output. You will need the instance ID when you call instance management or Spark application management APIs. See Spark application REST