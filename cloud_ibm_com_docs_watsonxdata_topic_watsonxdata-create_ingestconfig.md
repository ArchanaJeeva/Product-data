﻿IBM Cloud Docs Skip to contentIBM CloudCatalogCatalogCost EstimatorCost EstimatorHelpHelpDocsLog inSign upError Skip to content IBM Cloud IBM Cloud CatalogCatalog CatalogCatalog Cost EstimatorCost Estimator Cost EstimatorCost Estimator HelpHelpDocs HelpHelp Docs Docs Docs Log in Log in Sign up Sign up Error Config file ingestion in Presto ingestion mode Config file ingestion in Presto ingestion mode You can run the ibm-lh tool to ingest data into IBMÂ® watsonx.data through the CLI. The configuration file and examples are listed in this topic. Before you begin: Set the mandatory environment variable ENABLED\_INGEST\_MODE to PRESTO before starting an ingestion job by running the following command: export ENABLED\_INGEST\_MODE=PRESTO Set the environment variables for SOURCE\_S3\_CREDS and STAGING\_S3\_CREDS based on the requirements before starting an ingestion job by running the following commands: export SOURCE\_S3\_CREDS="AWS\_ACCESS\_KEY\_ID=,AWS\_SECRET\_ACCESS\_KEY=,ENDPOINT\_URL=,AWS\_REGION=,BUCKET\_NAME=" export STAGING\_S3\_CREDS="AWS\_ACCESS\_KEY\_ID=,AWS\_SECRET\_ACCESS\_KEY=,ENDPOINT\_URL=,AWS\_REGION=,BUCKET\_NAME=" About this task To run the ingestion jobs, you can use the configuration file option. Advantage of using a configuration file is that, multiple ingestion jobs can be completed in a single starting of the ingestion tool. Run the following command to do multiple ingestion jobs after you update the configuration file: ibm-lh data-copy --ingest-config / The commands must be run within the ibm-lh container. For more details and instructions to install ibm-lh-client package and

use the ibm-lh tool for ingestion, see Installing ibm-lh-client and Setting up the ibm-lh command-line utility. To access IBM Cloud Object Storage (COS) and MinIO object storage, specify the ENDPOINT\_URL to pass the corresponding url to the tool. For more information about IBM COS, see Endpoints and storage locations. Replace the absolute values inside angular brackets of command examples with values applicable to your environment. See Options and variables supported in ibm-lh tool. Following are the details of the config file option to ingest data files from S3 or local location to watsonx.data

Iceberg table: Ingest a single CSV/Parquet file from S3 location by using config file To ingest a single Parquet file from a S3 location, run the following command: [global-ingest-config] target-table:table\_name ingestion-engine:hostname=,port= create-if-not-exist: [ingest-config1] source- files:SOURCE\_DATA\_FILE staging-location:STAGING\_LOCATION For example: [global-ingest-config] target- table:iceberg\_cat.ice\_schema.customer1\_tab ingestion-engine:hostname=localhost,port=8080 create-if-not-exist:true [ingest-config1] source-files:s3://cust- bucket/warehouse/a\_source\_file.parquet staging-location:s3://cust-bucket/warehouse/staging/ Ingest multiple CSV/Parquet files and CSV folders from S3 location by using config file To ingest multiple Parquet files from a S3 location, run the following command: [global-ingest-config] target-table:table\_name ingestion-engine:hostname=,port= create-if-not-exist: [ingest-config1] source-files:SOURCE\_DATA\_FILE staging-location:STAGING\_LOCATION For example: [global-ingest-config] target-table:iceberg\_cat.ice\_schema.customer1\_tab ingestion-engine:hostname=localhost,port=8080 create-if-not-exist:true [ingest-config1] source-files:s3://cust-bucket/warehouse/a\_source\_file1.csv,s3://cust-bucket/warehouse/a\_source\_file2.csv staging-location:s3://cust- bucket/warehouse/staging/ [global-ingest-config] target-table:iceberg\_cat.ice\_schema.customer1\_tab ingestion-engine:hostname=localhost,port=8080 create-if-not-exist:true [ingest-config1] source-files:s3://cust-bucket/warehouse/ staging-location:s3://cust-bucket/warehouse/staging/ Ingest all Parquet files in a folder from S3 location by using config file To ingest all Parquet files in a folder from a S3 location, run the following command: [global-ingest-config] target-table:table\_name ingestion-engine:hostname=,port= create-if-not-exist: [ingest-config1] source-files:SOURCE\_DATA\_FILE For example: [global- ingest-config] target-table:iceberg\_cat.ice\_schema.customer1\_tab ingestion-engine:hostname=localhost,port=8080 create-if-not-exist:true [ingest-config1] source-files:s3://cust-bucket/warehouse/ In general, this option does not require a staging location. However, a few exceptional scenarios are there when a staging location must be specified. When the staging location is not used, make sure that the hive catalog configured with Presto can be used with source- files location. The following are the exceptional cases where a staging location is required: Any or all parquet files in the folder are huge. Any or all parquet files in the folder have special columns, such as TIME. Ingest a CSV/Parquet file or a folder of files from a local file system by using config file To ingest a single CSV file from a local location, run the following command: [global-ingest-config] target-table:table\_name ingestion-engine:hostname=,port= create-if- not-exist: [ingest-config1] source-files:SOURCE\_DATA\_FILE staging-location:STAGING\_LOCATION For example: [global-ingest-config] target- table:iceberg\_cat.ice\_schema.customer1\_tab ingestion-engine:hostname=localhost,port=8080 create-if-not-exist:true [ingest-config1] source- files:/tmp/customer1.parquet staging-location:s3://cust-bucket/warehouse/staging/ [global-ingest-config] target-table:iceberg\_cat.ice\_schema.customer1\_tab ingestion-engine:hostname=localhost,port=8080 create-if-not-exist:true [ingest-config1] source-files:/tmp/ staging-location:s3://cust- bucket/warehouse/staging/ Ingest any data file from local file system by using a config file To ingest any data file from a local location, run the following command: To ingest any type of data files from a local file system, data files are needed to be copied to ~ /ibm-lh-client/localstorage/volumes/ibm-lh directory. Now, you can access data files from /ibmlhdata/ directory by using the ibm-lh data-copy command. [global-ingest-config] target- table:table\_name ingestion-engine:hostname=,port= create-if-not-exist: [ingest-config1] source-files:SOURCE\_DATA\_FILE staging- location:STAGING\_LOCATIONstaging-hive-catalog: schema: dbuser: dbpassword: trust-store-path: trust-store-password: For example: [global-ingest- config] target-table:iceberg\_data.ivt\_sanity\_test\_1.reptile ingestion-engine:hostname=ibm-lh-lakehouse-presto-01-presto-svc-cpd- instance.apps.ivt384.cp.fyre.ibm.com,port=443 create-if-not-exist:true [ingest-config1] source-files:/ibmlhdata/reptile.csv staging- location:s3://watsonx.data/staging staging-hive-catalog:hive\_test schema:schema.cfg dbuser:xxxx dbpassword:xxxx trust-store- path:/mnt/infra/tls/aliases/ibm-lh-lakehouse-presto-01-presto-svc-cpd-instance.apps.ivt384.cp.fyre.ibm.com:443.crt trust-store-password:changeit Ingest CSV/local Parquet/S3 Parquet files that use staging location. To ingest CSV/local Parquet/S3 Parquet files that use staging location: [global-ingest-config] target-table:table\_name ingestion-engine:hostname=,port= create-if-not-exist: [ingest-config1] source-files:SOURCE\_DATA\_FILE staging- location:STAGING\_LOCATION staging-hive-catalog: schema: dbuser: dbpassword: trust-store-path: trust-store-password: For example: [global-ingest- config] target-table:iceberg\_data.test\_iceberg.gvt\_data\_v ingestion-engine:hostname=ibm-lh-lakehouse-presto-01-presto-svc-cpd- instance.apps.ivt384.cp.fyre.ibm.com,port=443 create-if-not-exist:true [ingest-config1] source-files:s3://watsonx-data-0823-2/test\_icos/GVT-DATA- C.csv staging-location:s3://watsonx.data-staging staging-hive-catalog:staging\_catalog staging-hive-schema:staging\_schema dbuser:xxxx dbpassword:xxxx trust-store-path:/mnt/infra/tls/aliases/ibm-lh-lakehouse-presto-01-presto-svc-cpd-instance.apps.ivt384.cp.fyre.ibm.com:443.crt trust-store- password:changeit Here, --staging-location is s3://watsonx.data-staging. The --staging-hive-catalog that is staging\_catalog must be associated with the bucket watsonx.data-staging. Config file ingestion in Presto ingestion mode You can run the ibm-lh tool to ingest data into IBMÂ® watsonx.data through the CLI. The configuration file and examples are listed in this topic. Before you begin: Set the mandatory environment variable ENABLED\_INGEST\_MODE to PRESTO before starting an ingestion job by running the following command: Set the environment variables for SOURCE\_S3\_CREDS and STAGING\_S3\_CREDS based on the requirements before starting an ingestion job by running the following commands:

About this task To run the ingestion jobs, you can use the configuration file option. Advantage of using a configuration file is that, multiple ingestion jobs can be completed in a single starting of the ingestion tool. Run the following command to do multiple ingestion jobs after you update the configuration file: The commands must be run within the ibm-lh container. For more details and instructions to install ibm-lh-client package and use the ibm-lh tool for ingestion,

see Installing ibm-lh-client and Setting up the ibm-lh command-line utility. Installing ibm-lh-client Setting up the ibm-lh command-line utility To access IBM Cloud Object Storage (COS) and MinIO object storage, specify the ENDPOINT\_URL to pass the corresponding url to the tool. For more information about IBM COS, see Endpoints and storage locations. Endpoints and storage locations Replace the absolute values inside angular brackets of command examples with values applicable to your environment. See Options and variables supported in ibm-lh tool. Options and variables supported in ibm-lh tool Following are the details of the config file option to ingest data files from S3 or local location to watsonx.data Iceberg table: Ingest a single CSV/Parquet file from S3 location by using config file To ingest a single Parquet file from a S3 location, run the following command: For example: Ingest multiple CSV/Parquet files and CSV folders from S3 location by using config file To ingest multiple Parquet files from a S3 location, run the following command: For example: Ingest all Parquet files in a folder from S3 location by using config file To ingest all Parquet files in a folder from a S3 location, run the following command: For example: In general, this option does not require a staging location. However, a few exceptional scenarios are there when a staging location must be specified. When the staging location is not used, make sure that the hive catalog configured with Presto can be used with source-files location. The following are the exceptional cases where a staging location is required: Any or all parquet files in the folder are huge. Any or all parquet files in the folder have special columns, such as TIME. Ingest a CSV/Parquet file or a folder of files from a local file system by using config file To ingest a single CSV file from a local location, run the following command: For example: Ingest any data file from local file system by using a config file To ingest any data file from a local location, run the following command: To ingest any type of data files from a local file system, data files are needed to be copied to ~ /ibm- lh-client/localstorage/volumes/ibm-lh directory. Now, you can access data files from /ibmlhdata/ directory by using the ibm-lh data-copy command. For example: Ingest CSV/local Parquet/S3 Parquet files that use staging location. To ingest CSV/local Parquet/S3 Parquet files that use staging location: For example: Here, --staging-location is s3://watsonx.data-staging. The --staging-hive-catalog that is staging\_catalog must be associated with the bucket watsonx.data-staging.