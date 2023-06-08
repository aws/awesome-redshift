# Awesome Redshift [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of awesome Amazon Redshift libraries, utilities, and resources.

- [Awesome Redshift](#awesome-redshift)
    - [General Workshops](#general-workshops)
    - [Key Features](#key-features)
        - [Amazon Redshift Serverless](#amazon-redshift-serverless)
        - [Data Sharing](#data-sharing)
        - [Data APIs](#data-apis)
        - [Federated Queries](#federated-queries)
        - [Streaming Ingestion](#streaming-ingestion)
        - [Redshift Spectrum](#redshift-spectrum)
        - [User Defined Functions (UDFs)](#user-defined-functions-udfs)
        - [Machine Learning (ML)](#machine-learning-ml)
    - [Performance Tuning](#performance-tuning)
    - [Connectors and Drivers](#connectors-and-drivers)
    - [Operations](#operations)
    - [Integrations](#integrations)
        - [Pandas](#pandas)
        - [dbt](#dbt)
        - [Grafana](#grafana)
        - [Apache Airflow](#apache-airflow)
        - [SQLAlchemy](#sqlalchemy)
        - [Querybook](#querybook)
        - [AWS Glue](#aws-glue)
        - [Amazon Location Service](#amazon-location-service)
    - [Security and Authentication](#security-and-authentication)
        - [General Security](#general-security)
        - [Single Sign On (SSO)](#single-sign-on-sso)
        - [Role Based Access Control (RBAC)](#role-based-access-control-rbac)
        - [Row Level Security (RLS)](#row-level-security-rls)
        - [Encryption](#encryption)
    - [Cost Optimization](#cost-optimization)
    - [CI/CD](#cicd)
    - [Redshift Internals](#redshift-internals)
- [General Resources](#general-resources)
- [Contributing](#contributing)

---

## General Workshops

*Hands-on workshops to learn Redshift.*

* [Amazon Redshift Deep Dive Workshop](https://catalog.us-east-1.prod.workshops.aws/workshops/380e0b8a-5d4c-46e3-95a8-82d68cf5789a/en-US) - A hands-on workshop covering topics such as: Data API, Spectrum,  Redshift ML, Lambda UDF, Query federation, SageMaker, Apache Hudi, QuickSight, PowerBI, Oracle/SQL Server migrations.
* [Redshift Immersion Labs Workshop](https://catalog.us-east-1.prod.workshops.aws/workshops/9f29cdba-66c0-445e-8cbb-28a092cb5ba7/en-US) - A hands-on workshop covering topics such as: ELT, Materialized Views, Data Sharing, and Redshift ML.

## Key Features

### Amazon Redshift Serverless
*[Amazon Redshift Serverless](#https://docs.aws.amazon.com/redshift/latest/mgmt/serverless-whatis.html) resources*
* [Amazon Redshift Serverless RSQL ETL Framework](https://github.com/aws-samples/amazon-redshift-serverless-rsql-etl-framework) - A Serverless ETL framework.
* [Self-service analytics with Amazon Redshift Serverless](https://www.youtube.com/watch?v=zGTxxOk4cBk) - A video session on getting started and best practices with Redshift Serverelss. 

### Data Sharing

*[Data Sharing](https://docs.aws.amazon.com/redshift/latest/dg/datashare-overview.html) for sharing data between Redshift clusters*

* [Seamless Data Sharing Using Amazon Redshift](https://catalog.us-east-1.prod.workshops.aws/workshops/4b2fb166-b467-461b-bd30-782dd2a2265c/en-US) - A hands-on workshop to share live data across Amazon Redshift clusters.
* [Optimize Data Pattern using Data Sharing](https://www.wellarchitectedlabs.com/sustainability/300_labs/300_optimize_data_pattern_using_redshift_data_sharing/) - A hands-on workshop using data sharing to reduce the provisioned storage required to support your workload.

### Data APIs

*Resources related to [Data APIs](https://docs.aws.amazon.com/redshift/latest/mgmt/data-api.html) for accessing Redshift from web services–based applications*

* [Getting Started with Redshift Data API](https://github.com/aws-samples/getting-started-with-amazon-redshift-data-api) - A sample project to access Redshift Data API from AWS Lambda.

### Federated Queries 

*Resources related to [Federated Queries](https://docs.aws.amazon.com/redshift/latest/dg/federated-overview.html) querying live data from external databases*

* [Best Practices for Amazon Redshift Federated Queries](https://aws.amazon.com/blogs/big-data/amazon-redshift-federated-query-best-practices-and-performance-considerations/) - A blog post listing  best practices to apply when using Redshift Federated Queries. 

### Streaming Ingestion

*Resources related to [Streaming Ingestion](https://docs.aws.amazon.com/redshift/latest/dg/materialized-view-streaming-ingestion.html) querying stream data from Amazon Kinesis Data Streams and Amazon Managed Streaming for Apache Kafka*

* [Real-time Analytics with Amazon Redshift Streaming Ingestion](https://aws.amazon.com/blogs/big-data/real-time-analytics-with-amazon-redshift-streaming-ingestion/) - A blog post describing how to query stream data in the same account.
* [Near Real-time Fraud Detection using Amazon Redshift Streaming Ingestion](https://aws.amazon.com/blogs/big-data/near-real-time-fraud-detection-using-amazon-redshift-streaming-ingestion-with-amazon-kinesis-data-streams-and-amazon-redshift-ml/) - A blog post describing how to use Amazon Redshift Streaming Ingestion, Amazon Kinesis Data Streams, and Amazon Redshift ML to detect fraud near real-time.
* [Cross-Account Streaming Ingestion for Amazon Redshift](https://aws.amazon.com/blogs/big-data/cross-account-streaming-ingestion-for-amazon-redshift/) - A blog post describing how to query stream data across accounts.
* [Amazon Redshift Streaming Workshop](https://github.com/aws-samples/amazon-redshift-streaming-workshop) - A hands-on workshop and sample library to build a near-realtime logistics dashboard using Amazon Redshift and Amazon Managed Grafana.

### Redshift Spectrum

*Resources related to [Redshift Spectrum](https://docs.aws.amazon.com/redshift/latest/dg/c-getting-started-using-spectrum.html) for querying S3 data*

* [Redshift Spectrum Row and Cell Level Security](https://aws.amazon.com/blogs/big-data/use-amazon-redshift-spectrum-with-row-level-and-cell-level-security-policies-defined-in-aws-lake-formation/) - A blog post describing how to use row and cell level security defined in AWS Lake Formation.

### User Defined Functions (UDFs)

*Collections of [User defined functions (UDFs)](https://docs.aws.amazon.com/redshift/latest/dg/user-defined-functions.html)*

* [UDFs Collection](https://github.com/aws-samples/amazon-redshift-udfs) - A collection of useful UDFs, such as bitwise ops, url parsing, masking, kms encryption, dynamodb lookups, and converting json to upper case.
* [Text UDFs](https://github.com/aws-samples/aws-redshift-udfs-textanalytics) - UDFs to analyze text, such as translating, detecting language, detecting sentiment, detecting and redacting entities, detecting and redacting PII.

### Machine Learning (ML)
*Resources related to [Amazon Redshift ML](https://aws.amazon.com/redshift/features/redshift-ml/)*

* [Create and train ML Models using Amazon Redshift ML](https://catalog.us-east-1.prod.workshops.aws/workshops/4efa7f96-66a8-4b39-b7ea-c34595b2352b/en-US) - A hands-on workshop using Redshift ML to predict customer churn.
* [Streaming Ingestion and ML Predictions with Amazon Redshift](https://catalog.us-east-1.prod.workshops.aws/workshops/03a761e3-8c64-42b6-8cc4-2123ffd1ec24/en-US) - A hands-on workshop using Streaming Ingestion and Redshift ML to detect fraud near real-time.

## Performance Tuning

*Tools and tips to measure and tune Redshift's performance.*

* [Top 10 Redshift Performance Tuning Techniques](https://aws.amazon.com/blogs/big-data/top-10-performance-tuning-techniques-for-amazon-redshift/) - A blog post outlining performance tuning techniques.
* [Test Drive](https://github.com/aws/redshift-test-drive) - A collection of utilities and automation to compare performance of different Redshift configurations for a given workload.
* [Simple Replay](https://github.com/awslabs/amazon-redshift-utils/tree/master/src/SimpleReplay) - A library to record your queries and replay them on a different cluster to test performance. (DEPRECATED: Use [Test Drive](https://github.com/aws/redshift-test-drive))
* [Node Configuration Compare](https://github.com/aws-samples/amazon-redshift-config-compare) - A library to compare performance of different cluster sizes and configurations by recording and replaying your queries (uses Simple Replay under the hood). (DEPRECATED: Use [Test Drive](https://github.com/aws/redshift-test-drive))
* [Admin Scripts](https://github.com/awslabs/amazon-redshift-utils/tree/master/src/AdminScripts) - A collection of queries and scripts to inspect performance and other administrative tasks.
* [Admin Views](https://github.com/awslabs/amazon-redshift-utils/tree/master/src/AdminViews) - A collection of views to inspect performance and other adminstrative tasks.
* [Benchmark Redshift Using TPC-DS and TPC-H](https://github.com/awslabs/amazon-redshift-utils/tree/master/src/CloudDataWarehouseBenchmark) - A collection of commands and queries to setup and run TPC-DS/TPC-H on Redshift.
* [The adx-tpc-ds Benchmark Scripts](https://github.com/aws-samples/redshift-benchmarks/tree/main/adx-tpc-ds) - A library to benchmark Redshift without having to generate and load data 
* [ClickBench - Compare Analytical DBMS](https://benchmark.clickhouse.com/) - A comparison of performance of various data warehouses and analytical DBMS.

## Connectors and Drivers
*Redshift connectors and drivers*
* [Amazon Redshift Python Driver](https://github.com/aws/amazon-redshift-python-driver) - Amazon Redshift's connector for Python.
* [Amazon Redshift JDBC driver](https://github.com/aws/amazon-redshift-jdbc-driver) - Amazon Redshift JDBC driver.
* [Amazon Redshift ODBC driver](https://github.com/aws/amazon-redshift-odbc-driver) - Amazon Redshift ODBC driver.
* [Amazon Redshift Integration with Apache Spark on EMR and Glue](https://aws.amazon.com/blogs/aws/new-amazon-redshift-integration-with-apache-spark/) - Connecting to Redshift from Amazon EMR 6.9, EMR Serverless, and AWS Glue 4.0.
* [Redshift Data Source for Apache Spark - Community Edition](https://github.com/spark-redshift-community/spark-redshift) - Connecting to Redshift from Apache Spark - community edition.
* [Query Amazon Redshift with Databricks](https://docs.databricks.com/external-data/amazon-redshift.html) - Connecting to Redshift from Databricks Runtime.

## Operations

*Tools and scripts to automate management and operations of Redshift.*

* [Visualize Redshift Operational Metrics Using Grafana](https://aws.amazon.com/blogs/big-data/query-and-visualize-amazon-redshift-operational-metrics-using-the-amazon-redshift-plugin-for-grafana/) - A blog post how to use Amazon Redshift plugin for Grafana to query and visualize Redshift operational metrics.
* [Redshift Stored Procedures](https://github.com/aws-samples/amazon-redshift-udfs/tree/master/stored-procedures) - A collection of stored procedures to perform common data tasks, such as integrity checks, permissions, and changing your data model.
* [Redshift Automation](https://github.com/awslabs/amazon-redshift-utils/tree/master/src/RedshiftAutomation) - A library to automate common tasks using AWS CloudWatch events and AWS Lambda.
* [QMR Notifications Utility](https://github.com/awslabs/amazon-redshift-utils/tree/master/src/QMRNotificationUtility) - A library to set SNS notifications for changes in WLM Query Monitoring Rules (QMR).

## Integrations

*Libraries and resources to help integrate Redshift with other frameworks and AWS services* 
### [Pandas](https://pandas.pydata.org/)
* [AWS SDK for Pandas](https://github.com/aws/aws-sdk-pandas) - A library to transfer data between [Pandas](https://pandas.pydata.org/), Redshift, and other AWS services.

### [dbt](https://docs.getdbt.com/reference/resource-configs/redshift-configs)
* [Best Practices for Leveraging Amazon Redshift and dbt](https://d1.awsstatic.com/products/Redshift/Amazon-Redshift-dBT-Best-Practice_paper.pdf) - A white-paper covering best practices and performance tuning when using dbt and Amazon Redshift.
* [Using DBT with Amazon Redshift Workshop](https://catalog.workshops.aws/dbt-cli-and-amazon-redshift/en-US) - A hands on workshop on integrating [DBT](https://github.com/dbt-labs/dbt-redshift) and Redshift.

### [Grafana](https://grafana.com)
* [Amazon Redshift Plugin for Grafana](https://grafana.com/grafana/plugins/grafana-redshift-datasource/) - Redshift plugin for Grafana.

### [Apache Airflow](https://airflow.apache.org/docs/apache-airflow-providers-amazon/stable/connections/redshift.html)
* [Amazon Redshift SQL Operator](https://airflow.apache.org/docs/apache-airflow-providers-amazon/2.4.0/operators/redshift.html) - An operator allowing Apache Airflow users to execute statements against Redshift in workflows.

### [SQLAlchemy](https://www.sqlalchemy.org/)
* [Use the Amazon Redshift SQLAlchemy dialect to interact with Amazon Redshift](https://aws.amazon.com/blogs/big-data/use-the-amazon-redshift-sqlalchemy-dialect-to-interact-with-amazon-redshift/) - A blog covering how to use the `sqlalchemy-redshift` dialect with SQLAlchemy.

### [Querybook](https://www.querybook.org/)
* [Adding Amazon Redshift Query engine to Querybook](https://www.querybook.org/docs/setup_guide/connect_to_query_engines/#step-by-step-guide) - A step by step guide showing how to add a Amazon Redshift query engine to Querybook.

### [AWS Glue](https://aws.amazon.com/glue/)
* [Execute Amazon Redshift Commands using AWS Glue](https://github.com/aws-samples/amazon-redshift-commands-using-aws-glue) - A library to use a AWS Glue Python Shell Job to execute SQL scripts on Amazon Redshift.

### [Amazon Location Service](https://aws.amazon.com/location/)
* [Amazon Redshift User Defined Functions to Call Amazon Location Service APIs](https://github.com/aws-samples/amazon-redshift-location-user-defined-functions) - A library using Lambda-based User Defined Functions (UDF) to call Amazon Location Service APIs.

## Security and Authentication
### General Security
*General resources for Redshift's security*
* [AWS Summit NY 2022 - Amazon Redshift Security Enhancements](https://www.youtube.com/watch?v=PPbmGLmivOA) - A video session covering authentication, access control, audit, and encryption.
* [AWS Config Rules for Redshift Security](https://github.com/awslabs/aws-config-rules/blob/master/aws-config-conformance-packs/Security-Best-Practices-for-Redshift.yaml) - An [AWS Config Rules](https://docs.aws.amazon.com/config/latest/developerguide/evaluate-config.html) [conformance pack](https://docs.aws.amazon.com/config/latest/developerguide/conformance-packs.html) to apply Amazon Redshift's security best practices.

### Single Sign On (SSO)
*Integration with SSO providers*

* [Integrate Amazon Redshift with Microsoft Azure AD](https://aws.amazon.com/blogs/big-data/integrate-amazon-redshift-native-idp-federation-with-microsoft-azure-ad-using-a-sql-client/) - A blog post describing how to integrate Amazon Redshift native IdP federation with Microsoft Azure AD using a SQL client.
* [Federate Amazon Redshift Access with Microsoft Azure AD SSO](https://aws.amazon.com/blogs/big-data/federate-amazon-redshift-access-with-microsoft-azure-ad-single-sign-on/) - A blog post describing how to federate Amazon Redshift access with Microsoft Azure AD single sign-on.
* [Federate SSO Access to Amazon Redshit with Okta](https://aws.amazon.com/blogs/big-data/federate-single-sign-on-access-to-amazon-redshift-query-editor-v2-with-okta/) - A blog post describing how to federate single sign-on access to Amazon Redshift query editor v2 with Okta.
* [Federate Access to Your Amazon Redshift cluster with Active Directory Federation Services](https://aws.amazon.com/blogs/big-data/federate-access-to-your-amazon-redshift-cluster-with-active-directory-federation-services-ad-fs-part-1/) - A 3-part blog post describing how to federate access to Amazon Redshift cluster with Active Directory Federation Services (AD FS).

### Role Based Access Control (RBAC)
*Using role-based access control (RBAC) to manage database permissions*
* [Simplify Management of Database Privileges in Amazon Redshift](https://aws.amazon.com/blogs/big-data/simplify-management-of-database-privileges-in-amazon-redshift-using-role-based-access-control/) - A blog post providing a step-by-step guide to setting up role based access control.
* [Introducing Role Based Access Control (RBAC) in Amazon Redshift](https://www.youtube.com/watch?v=IhHQ7mZ-tp4) - A video providing an overview and step-by-step guide to setting up role based access control.

### Row Level Security (RLS)
*Using row-level security (RLS) to gain granular access control*
* [Achieve Fine-Grained Data Security with Row-Level Access Control](https://aws.amazon.com/blogs/big-data/achieve-fine-grained-data-security-with-row-level-access-control-in-amazon-redshift/) - A blog post providing a step-by-step guide to setting up row level security.
* [AWS Summit NY 2022 - Amazon Redshift Security Enhancements](https://www.youtube.com/watch?v=PPbmGLmivOA) - A video session explaining how to protect data with role-based access controls, row-level security, and other AWS security features.

### Encryption
*Protect your data using encryption*
* [Encrypt Amazon Redshift Data Loads with Amazon S3 and AWS KMS](https://aws.amazon.com/blogs/big-data/encrypt-your-amazon-redshift-loads-with-amazon-s3-and-aws-kms/) - A blog post describing how to encrypted data loads end-to-end.
* [Accelerate Resize and Encryption of Amazon Redshift Clusters with Asynchronous Resize](https://aws.amazon.com/blogs/big-data/accelerate-resize-and-encryption-of-amazon-redshift-clusters-with-asynchronous-classic-resize/) - A blog post how to asynchronously resize and encrypt an existing cluster.

## Cost Optimization
*Tools and resources to help reduce Redshift cost*
* [Cost Optimization Guidelines for Amazon Redshift](https://d1.awsstatic.com/whitepapers/amazon-redshift-cost-optimization.pdf) - A white paper of best-practices to optimize Redshift's cost.
* [Query to Analyze Redshift's Cost and Usage Report (CUR)](https://wellarchitectedlabs.com/cost/300_labs/300_cur_queries/queries/database/#amazon-redshift) - SQL query to analyze analyze Redshift's cost and usage using Amazon Athena.
* [How to Attribute Amazon Redshift Costs to your End-Users](https://aws.amazon.com/blogs/big-data/how-to-attribute-amazon-redshift-costs-to-your-end-users/) - A blog detailing step-by-step instructions on how to attribute redshift costs to end users

## CI/CD

*Libraries and resources to help provision Redshift using CI/CD tools*

* [Apply CI/CD DevOps Principles to Amazon Redshift Development](https://aws.amazon.com/blogs/big-data/apply-ci-cd-devops-principles-to-amazon-redshift-development/) - A blog post and [accompanying repo](https://github.com/aws-samples/amazon-redshift-devops-blog) step by step guide to provision Redshift as a part of a deployment pipeline, using [AWS CodeCommit](https://aws.amazon.com/codecommit/), [AWS CodeBuild](http://aws.amazon.com/codebuild), and [AWS CodePipeline](http://aws.amazon.com/codepipeline).
* [Amazon Redshift Infrastructure Automation](https://github.com/aws-samples/amazon-redshift-infrastructure-automation) - A library to help automate provisoning of Redshift including data migration.
* [Terraform Redshift Example Module](https://github.com/cloudposse/terraform-aws-redshift-cluster) - A template repository to deploy Redshift using [Terraform](https://www.terraform.io/).
* [CDK Redshift Project](https://constructs.dev/packages/cdk-stepfunctions-redshift/) - An AWS Cloud Development Kit (CDK) [construct](https://docs.aws.amazon.com/cdk/v2/guide/constructs.html) to run SQL in Redshift using [AWS Step Functions](https://aws.amazon.com/step-functions).

## Redshift Internals
*Redshift's internal architecture and design*
* [Amazon Redshift Re-invented](https://www.amazon.science/publications/amazon-redshift-re-invented) - A paper outlining Redshift's internal system architecture, data organization, and query processing flow.

# General Resources

*Blogs, forums, and other online Redshift resources*

* [AWS re:Post](https://repost.aws/tags/TAByF7MpfSQUCX_lAeDTvODw/amazon-redshift) - A Q&A forum and knowledge sharing community.
* [AWS Big Data Blog](https://aws.amazon.com/blogs/big-data/category/database/amazon-redshift/) - AWS official data blog.
* [AWS Event YouTube Channel](https://www.youtube.com/@AWSEventsChannel/search?query=redshift) - Recorded presentations and talks from AWS events, such as re:Invent and AWS summits.

# Contributing

Your contributions are always welcome! Please take a look at the [contribution guidelines](https://github.com/aws/awesome-redshift/blob/main/CONTRIBUTING.md) first.

We will keep some pull requests open if we aren't sure whether those resources are awesome, you could [vote for them](https://github.com/aws/awesome-redshift/pulls) by adding :+1: to them.
