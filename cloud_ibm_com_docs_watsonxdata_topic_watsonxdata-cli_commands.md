﻿IBM Cloud Docs Skip to contentIBM CloudCatalogCatalogCost EstimatorCost EstimatorHelpHelpDocsLog inSign upError Skip to content IBM Cloud IBM Cloud CatalogCatalog CatalogCatalog Cost EstimatorCost Estimator Cost EstimatorCost Estimator HelpHelpDocs HelpHelp Docs Docs Docs Log in Log in Sign up Sign up Error Options and parameters supported in ibm-lh tool Options and parameters supported in ibm-lh tool Ingesting data files from S3 or local location into IBMÂ® watsonx.data is done by using the ibm-lh tool. The parameters supported in the ibm-lh tool is described in this topic. Before you begin: Set the mandatory environment variable for ENABLED\_INGEST\_MODE before starting an ingestion job in any mode of ingestion by running the following command: export ENABLED\_INGEST\_MODE=SPARK The different ingestion modes supported are PRESTO, SPARK\_LEGACY, and SPARK. The default mode is SPARK. Options and parameters Different options and variables that are supported in a ibm-lh tool invoked by ibm-lh data-copy command are listed as follows: Table 1. Command line options and variables Parameter Description Declaration Modes of ingestion create-if-not-exist Create target table if it does not exist. --create-if-not-exist PRESTO, SPARK\_LEGACY, and SPARK dbpassword Database password that is used to do ingestion. This is a mandatory parameter to run an ingestion job unless the default user is used. --dbpassword PRESTO dbuser Database username that is used to do ingestion. This is a mandatory parameter to run an ingestion job unless the default user is used. --dbuser PRESTO engine-id Engine id of Spark engine when using REST API based SPARK ingestion. The short command for this parameter is -e. --engine-id SPARK ingest-config Configuration file for data migration --ingest-config PRESTO and SPARK\_LEGACY ingestion-engine-endpoint Endpoint of ingestion engine. hostname=, port=. This is a mandatory parameter to run an ingestion job. --ingestion-engine-endpoint PRESTO and SPARK\_LEGACY instance-id Identify unique instances. In SaaS environment, CRN is the instance id. The short command for this parameter is -i. --instance-id SPARK job-id Job id is generated when REST API or UI based ingestion is initiated. This job id is used in getting the status of ingestion job. This parameter is used only used with ibm-lh get-status command. The short command for this parameter is -j ibm-lh get-status --job-id SPARK log-directory This option is used to specify the location of log files. See Log directory. --ingest-config --log-directory PRESTO, SPARK\_LEGACY, and SPARK password Password of the user connecting to the instance. In SaaS, API key to the isntance is used. The short command for this parameter is -pw. --password SPARK schema Schema file that includes CSV specifications, and more. See Schema file specifications. --schema PRESTO, SPARK\_LEGACY, and SPARK source-data-files Data files or folders for data migration. File name ending with / is considered a folder. Single or multiple files can be used. This is a mandatory parameter to run an ingestion job. Example: ,,. File names are case sensitive. The short command for this parameter is - s. --source-data-files PRESTO, SPARK\_LEGACY, and SPARK staging-location Location where CSV files and in some circumstances parquet files are staged, see Staging location. This is a mandatory parameter to run an ingestion job. --staging-location PRESTO staging-hive-catalog The hive catalog name configured in the watsonx.data if not using the default catalog for staging. Default catalog: hive\_data. --staging-hive-catalog PRESTO staging-hive-schema The schema name associated with the staging hive catalog for ingestion. Create and pass in a custom schema name by using this parameter. Default schema: lhingest\_staging\_schema. If schema is created as default, this parameter is not required. --staging-hive- schema PRESTO sync-status This parameter is used in REST API based ingestion. Default value is false. When this parameter is set to true, ibm- lh data-copy tool waits and polls to get continuous status after an ingestion job is submitted. --sync-status SPARK system-config This parameter is used to specify system related parameters. See System config. --system-config PRESTO, SPARK\_LEGACY, and SPARK target-catalog-uri Target catalog uri --target-catalog-uri SPARK\_LEGACY target-tables Data migration target table. ... This is a mandatory parameter to run an ingestion job. Example: . This parameter is deprecated and replaced with target-table. --target-tables PRESTO and SPARK\_LEGACY target- table Data migration target table. ... This is a mandatory parameter to run an ingestion job. Example: . The short command for this parameter is -t. See Target table. --target-table PRESTO, SPARK\_LEGACY, and SPARK trust-store-path Path of the truststore to access the ingestion engine. This is used to establish SSL connections. This is a mandatory parameter to run an ingestion job. --trust-store-path PRESTO and SPARK\_LEGACY trust-store-password Password of truststore to access the ingestion engine. This is used to establish SSL connections. This is a mandatory parameter to run an ingestion job. --trust-store-password PRESTO and SPARK\_LEGACY user User name of the user connecting to the instance. The short command for this parameter is -u. --user SPARK url Base url of the location of IBMÂ® watsonx.data cluster. The short command for this parameter is -w. --url SPARK System config The system-config parameter refers to a file and is used to specify system related parameters. For the command line, the parameter is declared as follows: --system-config /path/to/systemconfig/file The format of the system config parameter is as follows: [system-config] : : : ... Currently, only the memory-limit parameter is supported. This parameter specifies the maximum memory in watsonx.data that an ingestion job can use. Default value for memory-limit is 500M. The limit can be in bytes, K, M or G. The system- config is applicable for PRESTO, SPARK\_LEGACY, and SPARK ingestion modes. Following are some examples of how the memory-limit parameter can be specified in the system-config file. [system-config] memory-limit:500M [system-config] memory-limit:5000K [system-config] memory-limit:1G [system-config] memory-limit:10000000 #This is in bytes The memory-limit parameter is applicable for PRESTO ingestion mode. Staging location This parameter is applicable for PRESTO ingestion mode. The staging location is used for: CSV file or folder ingestion Local Parquet file or folder ingestion. S3 Parquet file ingestion In some circumstances, when the source file or files in the S3 Parquet folder contains special column types, such as TIME or are associated with different column types. For ingestion job through CLI, the staging bucket must be the same bucket that is associated with the Hive catalog. Staging is possible only in the Hive catalog. The internal MinIO buckets (iceberg-data, hive-data, wxd-milvus, wxd-system) and their associated catalogs cannot be used for staging, as their endpoints are not externally accessible. Users can use their own storage buckets that are exposed and accessible by external connections. Schema file specification The schema parameter points to the schema file. The schema file can be used to specify CSV file properties such as field delimiter, line delimiter, escape character, encoding and whether header exists in the CSV file. This parameter is applicable for PRESTO, SPARK\_LEGACY, and SPARK ingestion modes. The following is the schema file specification: [CSV] DELIMITER: #default ',' #LINE\_DELIMITER: #A single char delimiter other than ' '(blank), need not be enclosed in quotes. #Must be enclosed in quotes if it is one of: '\n' for newline, '\t' for TAB, ' ' for space. LINE\_DELIMITER: #default '\n' HEADER: #default 'true' #HEADER is a mandatory entry within schema file. #single character value ESCAPECHAR: #default '\\' #Example encodings: #utf-8, cp1252, iso-88509-1, latin1 etc ENCODING: #default None The following is an example of schema specification: $ more /tmp/schema.cfg [CSV] DELIMITER:, HEADER:false LINE\_DELIMITER:'\n' Log directory The ingest log files are generated in the log directory. By default, the ingest log file is generated as /tmp/ingest.log. By using the --log-directory parameter, you can specify a new location for ingest log files. A separate log file is created for each ingest command invocation. The new log file name is in the format ingest\_.log. The log directory must exist before invocation of the ibm-lh ingest tool. This parameter is applicable only in the command line option for PRESTO, SPARK\_LEGACY, and SPARK ingestion modes. Example when using the command line: ibm-lh data-copy --source-data- files s3://cust-bucket/warehouse/a\_source\_file1.csv,s3://cust-bucket/warehouse/a\_source\_file2.csv --staging-location s3://cust- bucket/warehouse/staging/ --target-table iceberg\_target\_catalog.ice\_schema.cust\_tab1 --ingestion-engine-endpoint "hostname=localhost,port=8080" --create-if-not-exist --log-directory /tmp/mylogs Example when using a config file: ibm-lh data-copy --ingest- config ext.cfg --log-directory /tmp/mylogs Target table The ability to handle special characters in table and schema names for ingestion is constrained by the underlying engines (Presto, Legacy Spark, Spark) and the special characters they support. When using schema or table names with special characters, not all special characters will be accepted or handled by Spark, Presto, Legacy Spark. Consult the documentation for the special characters support. The SQL identifier of the target table for data migration is ... Use double quotes " or backticks ` to escape parts with special characters. Examples: ibm-lh data-copy --target-table 'catalog."schema 2.0"."my table!"' ibm-lh data-copy --target-table 'catalog.schema 2.0.my table!' ibm-lh data-copy --target-table catalog.'"schema 2.0"'.'"my table!"' ibm-lh data-copy --target-table "catalog.\schema 2.0`.`my table!`"` ibm-lh data-copy --target-table catalog.\"schema\ 2.0\".\"my\ table!\" Both double quotes " and backticks ` are accepted, but quote styles cannot be mixed. In order to include a literal quote inside an identifier, double the quoting character (e.g., "" or ``). Options and parameters supported in ibm-lh tool Ingesting data files from S3 or local location into IBMÂ® watsonx.data is done by using the ibm-lh tool. The parameters supported in the ibm-lh tool is described in this topic. Before you begin: Set the mandatory environment variable for ENABLED\_INGEST\_MODE before starting an ingestion job in any mode of ingestion by running the following command: The different ingestion modes supported are PRESTO, SPARK\_LEGACY, and SPARK. The default mode is SPARK. Options and parameters Different options and variables that are supported in a ibm-lh tool invoked by ibm-lh data-copy command are listed as follows: create-if-not-exist Create target table if it does not exist. --create-if-not-exist PRESTO, SPARK\_LEGACY, and SPARK dbpassword Database password that is used to do ingestion. This is a mandatory parameter to run an ingestion job unless the default user is used. --dbpassword PRESTO dbuser Database username that is used to do ingestion. This is a mandatory parameter to run an ingestion job unless the default user is used. --dbuser PRESTO engine-id Engine id of Spark engine when using REST API based SPARK ingestion. The short command for this parameter is -e. --engine-id SPARK ingest-config Configuration file for data migration --ingest-config PRESTO and SPARK\_LEGACY ingestion-engine-endpoint Endpoint of ingestion engine. hostname=, port=. This is a mandatory parameter to run an ingestion job. --ingestion-engine-endpoint PRESTO and SPARK\_LEGACY instance- id Identify unique instances. In SaaS environment, CRN is the instance id. The short command for this parameter is -i. --instance-id SPARK job- id Job id is generated when REST API or UI based ingestion is initiated. This job id is used in getting the status of ingestion job. This parameter is used only used with ibm-lh get-status command. The short command for this parameter is -j ibm-lh get-status --job-id SPARK log-directory This option is used to specify the location of log files. See Log directory. Log directory --ingest-config --log-directory PRESTO, SPARK\_LEGACY, and SPARK password Password of the user connecting to the instance. In SaaS, API key to the isntance is used. The short command for this parameter is -pw. --password SPARK schema Schema file that includes CSV specifications, and more. See Schema file specifications. Schema file specifications --schema PRESTO, SPARK\_LEGACY, and SPARK source-data-files Data files or folders for data migration. File name ending with / is considered a folder. Single or multiple files can be used. This is a mandatory parameter to run an ingestion job. Example: ,,. File names are case sensitive. The short command for this parameter is -s. --source-data-files PRESTO, SPARK\_LEGACY, and SPARK staging- location Location where CSV files and in some circumstances parquet files are staged, see Staging location. This is a mandatory parameter to run an ingestion job. Staging location --staging-location PRESTO staging-hive-catalog The hive catalog name configured in the watsonx.data if not using the default catalog for staging. Default catalog: hive\_data. --staging-hive-catalog PRESTO staging-hive-schema The schema name associated with the staging hive catalog for ingestion. Create and pass in a custom schema name by using this parameter. Default schema: lhingest\_staging\_schema. If schema is created as default, this parameter is not required. --staging-hive-schema PRESTO sync-status This parameter is used in REST API based ingestion. Default value is false. When this parameter is set to true, ibm-lh data-copy tool waits and polls to get continuous status after an ingestion job is submitted. --sync-status SPARK system-config This parameter is used to specify system related parameters. See System config. System config --system-config PRESTO, SPARK\_LEGACY, and SPARK target-catalog-uri Target catalog uri - -target-catalog-uri SPARK\_LEGACY target-tables Data migration target table. ... This is a mandatory parameter to run an ingestion job. Example: . This parameter is deprecated and replaced with target-table. --target-tables PRESTO and SPARK\_LEGACY target-table Data migration target table. ... This is a mandatory parameter to run an ingestion job. Example: . The short command for this parameter is -t. See Target table. Target table --target-table PRESTO, SPARK\_LEGACY, and SPARK trust-store-path Path of the truststore to access the ingestion engine. This is used to establish SSL connections. This is a mandatory parameter to run an ingestion job. --trust-store-path PRESTO and SPARK\_LEGACY trust-store-password Password of truststore to access the ingestion engine. This is used to establish SSL connections. This is a mandatory parameter to run an ingestion job. --trust-store-password PRESTO and SPARK\_LEGACY user User name of the user connecting to the instance. The short command for this parameter is -u. --user SPARK url Base url of the location of IBMÂ® watsonx.data cluster. The short command for this parameter is -w. --url SPARK System config The system-config parameter refers to a file and is used to specify system related parameters. For the command line, the parameter is declared as follows: The format of the system config parameter is as follows: Currently, only the memory-limit parameter is supported. This parameter specifies the maximum memory in watsonx.data that an ingestion job can use. Default value for memory-limit is 500M. The limit can be in bytes, K, M or G. The system-config is applicable for PRESTO, SPARK\_LEGACY, and SPARK ingestion modes. Following are some examples of how the memory-limit parameter can be specified in the system-config file. The memory-limit parameter is applicable for PRESTO ingestion mode. Staging location This parameter is applicable for PRESTO ingestion mode. The staging location is used for: CSV file or folder ingestion Local Parquet file or folder ingestion. S3 Parquet file ingestion In some circumstances, when the source file or files in the S3 Parquet folder contains special column types, such as TIME or are associated with different column types. For ingestion job through CLI, the staging bucket must be the same bucket that is associated with the Hive catalog. Staging is possible only in the Hive catalog. The internal MinIO buckets (iceberg-data, hive-data, wxd-milvus, wxd-system) and their associated catalogs cannot be used for staging, as their endpoints are not externally accessible. Users can use their own storage buckets that are exposed and accessible by external connections. Schema file specification The schema parameter points to the schema file. The schema file can be used to specify CSV file properties such as field delimiter, line delimiter, escape character, encoding and whether header exists in the CSV file. This parameter is applicable for PRESTO, SPARK\_LEGACY, and SPARK ingestion modes. The following is the schema file specification: The following is an example of schema specification: Log directory The ingest log files are generated in the log directory. By default, the ingest log file is generated as /tmp/ingest.log. By using the --log-directory parameter, you can specify a new location for ingest log files. A separate log file is created for each ingest command invocation. The new log file name is in the format ingest\_.log. The log directory must exist before invocation of the ibm-lh ingest tool. This parameter is applicable only in the command line option for PRESTO, SPARK\_LEGACY, and SPARK ingestion modes. Example when using the command line: Example when using a config file: Target table The ability to handle special characters in table and schema names for ingestion is constrained by the underlying engines (Presto, Legacy Spark, Spark) and the special characters they support. When using schema or