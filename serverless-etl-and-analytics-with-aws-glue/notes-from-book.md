# OLTP & OLAP

Traditionally, data storage systems have been classified as Online Transaction Processing (OLTP) and Online Analytical Processing (OLAP). OLTP systems are responsible for day-to-day business executions.

# normalized data model

These faster updates are achieved by using a normalized data model. Normalization is the process of structuring the dataset as per a set of normal-forms to reduce redundancy and enhance data integrity. The normalized data model ensures that you don’t update multiple tables with the same information for a user operation.

This is done by reducing the redundancy of the data in these systems. For example, if a customer updates their preferred_name, we can make this change in one table; the rest of the dependent tables will use customer_id to fetch updated information. So, a typical SQL query for the CRM application that’s used by the customer service agent contains the customer_id = 'xxxxxx' expression or data_plan_id = 'xxxxxx' in the WHERE clause.

These OLTP systems are not designed for obtaining or analyzing trends – for example, a query for gathering the mobile data usage (volume) of all customers over the last 2 years. Such queries involve joining a lot of tables on the OLTP side because of normalizations and usually results in poor performance as the amount of data scales up.

This problem can be solved by using OLAP systems. OLAP systems typically use the data warehouse of an organization, where they are utilized for executing complex queries over a large amount of data. They generally store historical datasets.

# Data warehouses and data marts

In Inmon’s top-down data warehousing approach, data architects and modelers start by looking at the holistic data landscape of an organization and identifying the main subject areas and entities under it. Inmon’s data warehouse is normalized and avoids redundancy. This simplifies the data ingestion process but is not optimized for queries. Hence, data marts are built on top of data warehouses and users access these data marts for their queries.

While data marts can be based on a star or snowflake schema, the star schema is generally preferred because it results in faster queries due to fewer joins. In 1996, Ralph Kimball introduced the star schema methodology to the data management world. This follows the bottom-up approach and creates data marts based on the business requirements instead of starting with an enterprise data warehouse.

# Data lakes

A data lake can be defined as a centralized repository that allows you to store all structured and unstructured data at any scale. With today’s hyper scalers providing cheap and durable storage, it is now possible for organizations to store all of their data in the cloud without significant cost implications. Data lakes are broken down into layers or zones.

In the first layer of the data lake, data is generally stored as-is. This reduces the entry barrier and enables organizations to move all of their data to the “lake” without significantly increasing development or maintenance costs. Because the first layer of the data lake is an as-is copy of the data, organizations can use an automated configuration-based pipeline to create newer sources.

Organizations usually pick a replication tool such as AWS Data Migration Service (AWS DMS) to bring the data into the data lake. While AWS DMS involves taking care of the replication infrastructure, it is mostly a hands-off mechanism for hydrating the lake. Organizations may also use a push mechanism to FTP to transfer the files to an AWS Simple Storage Service (S3)-based data lake using AWS Transfer Family.

# Data mesh

While cheap, durable storage helped in storing vast volumes of data, this data had to be secured properly. Since data from a vast variety of sources is stored in the lake, it becomes difficult to define the ownership and management of this data. This requirement resulted in a paradigm of serving data as a product and setting the ownership of the product. This thought process led to the creation of the data mesh.

Data meshes ensure that data lakes don’t become another monolith that the organization’s IT teams now have to manage. This decentralization leads to the democratization of data, which fuels innovation without hindering access to the data. Although data is decentralized and offered as a service, the permission model that’s applied to create a data lake ensures interoperability to reduce the barriers to accessing data products for users that have the right permissions.

# AWS Glue

On August 14, 2017, AWS released a new service called AWS Glue. AWS Glue is a serverless data integration service. AWS Glue also provides some easy-to-use features that almost eliminate the administrative overhead of infrastructure management and simplify how common data integration tasks can be integrated.

Let’s look at some of the notable components of the AWS Glue feature set:

- AWS Glue DataBrew: Glue DataBrew is used for data cleansing and enrichment through another GUI. Creating AWS Glue DataBrew Jobs does not require the user to write any source code and the Jobs are created with the help of a GUI.

- AWS Glue Data Catalog: AWS Glue Data Catalog is a central catalog of metadata that can be used with other AWS services such as Amazon Athena, Amazon Redshift, and Amazon EMR.

- AWS Glue Connections: Glue Connections are catalog objects that help organize and store connection information to various data stores. AWS Glue Connections can also be created for Marketplace AWS Glue Connectors, which allows you to integrate with third-party data stores, such as Apache Hudi, Google Big Query, and Elastic Search.

- AWS Glue Crawlers: Crawlers can be used to crawl existing data and populate an AWS Glue Data Catalog with metadata.

- AWS Glue ETL Jobs: Glue ETL Jobs enables users to extract source data from various data stores, process it, and write output to a data target based on the logic defined in the ETL script. Users can take advantage of Apache Spark-based ETL Jobs to handle their workload in a distributed fashion. Glue also offers Python shell Jobs for ETL workloads; these don’t need distributed processing.

- AWS Glue Interactive Sessions: Interactive sessions are managed interactive environments that can be used to develop and test AWS Glue ETL scripts.

- AWS Glue Schema Registry: AWS Glue Schema Registry allows users to centrally control data stream schemas and has integrations with Apache Kafka, Amazon Kinesis, and AWS Lambda.

- AWS Glue Triggers: AWS Glue Triggers are data catalog objects that allow us to either manually or automatically start executing one or more AWS Glue Crawlers or AWS Glue ETL Jobs.

- AWS Glue Workflows: Glue Workflows can be used to orchestrate the execution of a set of AWS Glue Jobs and AWS Glue Crawlers using AWS Glue Triggers.

- AWS Glue Blueprints: Blueprints are useful for creating parameterized workflows that can be created and shared for similar use cases.

- AWS Glue Elastic Views: Glue Elastic Views helps users replicate the data from one store to another using familiar SQL syntax.

# Data integration

Data integration is a complex operation that involves several tasks – data discovery, ingestion, preparation, transformation, and replication. Data integration is the very first step in deriving insights from data so that data can be shared across the organization for collaboration and faster decision-making.
