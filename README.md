# Awesome Redshift [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of awesome Amazon Redshift libraries, utilities, and resources.

- [Awesome Redshift](#awesome-redshift)
    - [Workshops](#workshops)
    - [Connectors and Drivers](#connectors-and-drivers)
    - [Performance Tuning](#performance-tuning)
    - [Operations](#operations)
    - [UDFs](#udfs)
    - [Redshift Spectrum](#redshift-spectrum)
    - [Data Sharing](#data-sharing)
    - [Data APIs](#data-apis)
    - [Federated Queries](#federated-queries)
    - [Streaming Ingestion](#streaming-ingestion)
    - [Integarions](#integrations)
    - [Single Sign On (SSO)](#single-sign-on-sso)
    - [CI/CD](#cicd)
    - [Redshift Internals](#redshift-internals)
- [General Resources](#general-resources)
- [Contributing](#contributing)

---

## Workshops

*Hands-on workshops to learn Redshift.*

* [Amazon Redshift Deep Dive Workshop](https://catalog.us-east-1.prod.workshops.aws/workshops/380e0b8a-5d4c-46e3-95a8-82d68cf5789a/en-US) - A hands-on workshop covering topics such as: Data API, Spectrum,  Redshift ML, Lambda UDF, Query federation, SageMaker, Apache Hudi, QuickSight, PowerBI, Oracle/SQL Server migrations.
* [Redshift Immersion Labs Workshop](https://catalog.us-east-1.prod.workshops.aws/workshops/9f29cdba-66c0-445e-8cbb-28a092cb5ba7/en-US) - A hands-on workshop covering topics such as: ELT, Materialized Views, Data Sharing, and Redshift ML

## Connectors and Drivers
*Redshift connectors and drivers*
* [Amazon Redshift Python Driver](https://github.com/aws/amazon-redshift-python-driver) - Amazon Redshift's connector for Python
* [Amazon Redshift JDBC driver](https://docs.aws.amazon.com/redshift/latest/mgmt/jdbc20-download-driver.html) - Amazon Redshift JDBC driver version 2.1
* [Amazon Redshift ODBC driver](https://docs.aws.amazon.com/redshift/latest/mgmt/odbc20-install.html) - Amazon Redshift ODBC driver 
* [Amazon Redshift Integration with Apache Spark on EMR and Glue](https://aws.amazon.com/blogs/aws/new-amazon-redshift-integration-with-apache-spark/) - Connecting to Redshift from Amazon EMR 6.9, EMR Serverless, and AWS Glue 4.0
* [Redshift Data Source for Apache Spark - Community Edition](https://github.com/spark-redshift-community/spark-redshift) - Connecting to Redshift from Apache Spark - community edition
* [Query Amazon Redshift with Databricks](https://docs.databricks.com/external-data/amazon-redshift.html) - Connecting to Redshift from Databricks Runtime

## Performance Tuning

*Tools and tips to measure and tune Redshift's performance.*

* [Top 10 Redshift Performance Tuning Techniques](https://aws.amazon.com/blogs/big-data/top-10-performance-tuning-techniques-for-amazon-redshift/) - A blog post outlining performance tuning techniques.
* [Simple Replay](https://github.com/awslabs/amazon-redshift-utils/tree/master/src/SimpleReplay) - A library to record your queries and replay them on a different cluster to test performance.
* [Node Configuration Compare](https://github.com/aws-samples/amazon-redshift-config-compare) - A library to compare performance of different cluster sizes and configurations by recording and replaying your queries (uses Simple Replay under the hood).
* [Admin Scripts](https://github.com/awslabs/amazon-redshift-utils/tree/master/src/AdminScripts) - A collection of queries and scripts to inspect performance and other adminstrative tasks.
* [Admin Views](https://github.com/awslabs/amazon-redshift-utils/tree/master/src/AdminViews) - A collection of views to inspect performance and other adminstrative tasks.
* [Benchmark Redshift Using TPC-DS and TPC-H](https://github.com/awslabs/amazon-redshift-utils/tree/master/src/CloudDataWarehouseBenchmark) - A collection of commands and queries to setup and run TPC-DS/TPC-H on Redshift.
* [ClickBench - Compare Analytical DBMS](https://benchmark.clickhouse.com/) - A comparison of performance of various data warehouses and analytical DBMS.

## Operations

*Tools and scripts to automate management and operations of Redshift.*

* [Redshift Stored Procedures](https://github.com/aws-samples/amazon-redshift-udfs/tree/master/stored-procedures) - A collection of stored procedures to perform common data tasks, such as integrity checks, permissions, and changing your data model.
* [Redshift Automation](https://github.com/awslabs/amazon-redshift-utils/tree/master/src/RedshiftAutomation) - A library to automate common tasks using CloudWatch events and Lambda. 
* [QMR Notifications Utility](https://github.com/awslabs/amazon-redshift-utils/tree/master/src/QMRNotificationUtility) - A library to set SNS notifications for changes in WLM Query Monitoring Rules (QMR)

## UDFs

*Collections of User defined functions (UDFs)*

* [UDFs Collection](https://github.com/aws-samples/amazon-redshift-udfs) - A collection of useful UDFs, such as bitwise ops, url parsing, masking, kms encryption, dynamodb lookups, and converting json to upper case.
* [Text UDFs](https://github.com/aws-samples/aws-redshift-udfs-textanalytics) - UDFs to analyze text, such as translating, detecting language, detecting sentiment, detecting and redacting entities, detecting and redacting PII.

## Redshift Spectrum

*Resources related to Redshift Spectrum for querying S3 data*

* [Redshift Spectrum Row and Cell Level Security](https://aws.amazon.com/blogs/big-data/use-amazon-redshift-spectrum-with-row-level-and-cell-level-security-policies-defined-in-aws-lake-formation/) - A blog post describing how to use row and cell level security defined in AWS Lake Formation. 

## Data Sharing

*Resources related to Data Sharing for sharing data between Redshift clusters*

* [Seamless Data Sharing Using Amazon Redshift](https://catalog.us-east-1.prod.workshops.aws/workshops/4b2fb166-b467-461b-bd30-782dd2a2265c/en-US) - A hands-on workshop to share live data across Amazon Redshift clusters

## Data APIs

*Resources related to Data APIs for accessing Redshift from web services–based applications*

* [Getting Started with Redshift Data API](https://github.com/aws-samples/getting-started-with-amazon-redshift-data-api) - A sample project to access Redshift Data API from AWS Lambda.

## Federated Queries 

*Resources related to Federated Queries querying live data from external databases*

* [Best Practices for Amazon Redshift Federated Queries](https://aws.amazon.com/blogs/big-data/amazon-redshift-federated-query-best-practices-and-performance-considerations/) - A blog post listing  best practices to apply when using Redshift Federated Queries. 

## Streaming Ingestion

*Resources related to Streaming Ingestion querying stream data from Amazon Kinesis Data Streams and Amazon Managed Streaming for Apache Kafka*

* [Real-time Analytics with Amazon Redshift Streaming Ingestion](https://aws.amazon.com/blogs/big-data/real-time-analytics-with-amazon-redshift-streaming-ingestion/) - A blog post decribing how to query stream data in the same account.
* [Cross-Account Streaming Ingestion for Amazon Redshift](https://aws.amazon.com/blogs/big-data/cross-account-streaming-ingestion-for-amazon-redshift/) - A blog post decribing how to query stream data across accounts.
* [Amazon Redshift Streaming Workshop](https://github.com/aws-samples/amazon-redshift-streaming-workshop) - A hands-on workshop and sample library to build a near-realtime logistics dashboard using Amazon Redshift and Amazon Managed Grafana

## Integrations

*Libraries and resources to help integrate Redshift with other frameworks and AWS services* 

* [AWS SDK for Pandas](https://github.com/aws/aws-sdk-pandas) - A library to transfer data between [Pandas](https://pandas.pydata.org/), Redshift, and other AWS services
* [Execute Amazon Redshift Commands using AWS Glue](https://github.com/aws-samples/amazon-redshift-commands-using-aws-glue) - A library to use a AWS Glue Python Shell Job to execute SQL scripts on Amazon Redshift.
* [Amazon Redshift User Defined Functions to Call Amazon Location Service APIs](https://github.com/aws-samples/amazon-redshift-location-user-defined-functions) - A library using Lambda-based User Defined Functions (UDF) to call Amazon Location Service APIs.
* [Using DBT with Amazon Redshift Workshop](https://catalog.workshops.aws/dbt-cli-and-amazon-redshift/en-US) - A hands on workshop on integrating [DBT](https://github.com/dbt-labs/dbt-redshift) and Redshift.

## Single sign on (SSO)

*Integration with SSO providers*

* [Integrate Amazon Redshift with Microsoft Azure AD](https://aws.amazon.com/blogs/big-data/integrate-amazon-redshift-native-idp-federation-with-microsoft-azure-ad-using-a-sql-client/) - A blog post describing how to integrate Amazon Redshift native IdP federation with Microsoft Azure AD using a SQL client
* [Federate Amazon Redshift Access with Microsoft Azure AD SSO](https://aws.amazon.com/blogs/big-data/federate-amazon-redshift-access-with-microsoft-azure-ad-single-sign-on/) - A blog post describing how to federate Amazon Redshift access with Microsoft Azure AD single sign-on
* [Federate SSO Access to Amazon Redshit with Okta](https://aws.amazon.com/blogs/big-data/federate-single-sign-on-access-to-amazon-redshift-query-editor-v2-with-okta/) - A blog post describing how to federate single sign-on access to Amazon Redshift query editor v2 with Okta.
* [Federate Access to Your Amazon Redshift cluster with Active Directory Federation Services](https://aws.amazon.com/blogs/big-data/federate-access-to-your-amazon-redshift-cluster-with-active-directory-federation-services-ad-fs-part-1/) - A 3-part blog post describing how to federate access to Amazon Redshift cluster with Active Directory Federation Services (AD FS).

## CI/CD

*Libraries and resources to help provision Redshift using CI/CD tools*

* [Apply CI/CD DevOps Principles to Amazon Redshift Development](https://aws.amazon.com/blogs/big-data/apply-ci-cd-devops-principles-to-amazon-redshift-development/) - A blog post and [accompanying repo](https://github.com/aws-samples/amazon-redshift-devops-blog) step by step guide to provision Redshift as a part of a deployment pipeline, using [AWS CodeCommit](https://aws.amazon.com/codecommit/), [AWS CodeBuild](http://aws.amazon.com/codebuild), and [AWS CodePipeline](http://aws.amazon.com/codepipeline).
* [Amazon Redshift Infrastructure Automation](https://github.com/aws-samples/amazon-redshift-infrastructure-automation) - A library to help automate provisoning of Redshift including data migration
* [Terraform Redshift Example Module](https://github.com/cloudposse/terraform-aws-redshift-cluster) - A template repository to deploy Redshift using [Terraform](https://www.terraform.io/) 
* [CDK Redshift Project](https://constructs.dev/packages/cdk-stepfunctions-redshift/) - An AWS Cloud Development Kit (CDK) [construct](https://docs.aws.amazon.com/cdk/v2/guide/constructs.html) to run SQL in Redshift using [AWS Step Functions](https://aws.amazon.com/step-functions)

## Redshift Internals
*Redshift's internal architecture and design*
* [Amazon Redshift Re-invented](https://www.amazon.science/publications/amazon-redshift-re-invented) - A paper outlining Redshift's internal system architecture, data organization, and query
processing flow.

# General Resources

*Blogs, forums, and other online Redshift resources*

* [AWS re:Post](https://repost.aws/tags/TAByF7MpfSQUCX_lAeDTvODw/amazon-redshift) - A Q&A forum and knowledge sharing community.
* [AWS Big Data Blog](https://aws.amazon.com/blogs/big-data/category/database/amazon-redshift/) - AWS official data blog.
* [AWS Event YouTube Channel](https://www.youtube.com/@AWSEventsChannel/search?query=redshift) - Recorded presentations and talks from AWS events, such as re:Invent and AWS summits 

# Contributing

Your contributions are always welcome! Please take a look at the [contribution guidelines](https://github.com/aws/awesome-redshift/blob/main/CONTRIBUTING.md) first.

We will keep some pull requests open if we aren't sure whether those resources are awesome, you could [vote for them](https://github.com/aws/awesome-redshift/pulls) by adding :+1: to them. 
