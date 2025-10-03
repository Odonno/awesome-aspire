# Awesome .NET Aspire [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[<img src="dotnet-aspire-logo-256.svg" align="right" width="100">](https://github.com/dotnet/aspire)

Aspire provides tools, templates, and packages for building observable, production-ready distributed apps. Aspire gives you a unified toolchain: launch and debug your entire app locally with one command, then deploy anywhere—Kubernetes, the cloud, or your own servers—using the same composition.

Inspired by [awesome](https://github.com/sindresorhus/awesome), [awesome-dotnet](https://github.com/quozd/awesome-dotnet),  [awesome-dotnet-core](https://github.com/thangchung/awesome-dotnet-core).

Contributions are always welcome! Please take a look at the [contribution guidelines](https://github.com/Odonno/awesome-aspire/blob/main/contributing.md) pages first. We accept proprietary and commercial software too.

Thanks to all [contributors](https://github.com/Odonno/awesome-aspire/graphs/contributors), you're awesome and wouldn't be possible without you! The goal is to build a categorized community-driven collection of very well-known resources.

## Contents

* [General](#general)
* [Integrations](#integrations)
  * [AI](#ai)
  * [Authentication and Authorization](#authentication-and-authorization)
  * [AWS](#aws)
  * [Azure](#azure)
  * [Caching](#caching)
  * [Databases](#databases)
  * [Feature flags](#feature-flags)
  * [Logging](#logging)
  * [Mail](#mail)
  * [ORM](#orm)
  * [Programming languages](#programming-languages)
  * [Queue and Messaging](#queue-and-messaging)
  * [Storage](#storage)
  * [Testing](#testing)
  * [Tools](#tools)
* [Sample Projects](#sample-projects)
* [Videos](#videos)
* [Community](#community)

## General

* [dotnet/aspire](https://github.com/dotnet/aspire) - Main GitHub repository of the .NET Aspire project.
* [Aspire Community Toolkit](https://github.com/CommunityToolkit/Aspire) - A GitHub repository for community contributors to add integrations for .NET Aspire.
* [.NET Aspire documentation](https://learn.microsoft.com/en-us/dotnet/aspire/) - The official .NET Aspire documentation.
* [Aspire Roadmap (2025 → 2026)](https://github.com/dotnet/aspire/discussions/10644) - The current .NET Aspire Roadmap, going from 2025 to 2026.
* [Welcome to .NET Aspire](https://www.youtube.com/watch?v=UYH97nPLWrM&list=PLdo4fOcmZ0oUfIayQMrRqaSL55Rkck-GD) - A YouTube videos playlist to welcome developers into .NET Aspire.

## Integrations

### AI

* [AI Foundry](https://www.nuget.org/packages/Aspire.Hosting.Azure.AIFoundry) - Provides extension methods and resource definitions for a .NET Aspire AppHost to configure Azure AI Foundry.
* [Azure AI Inference](https://www.nuget.org/packages/Aspire.Azure.AI.Inference) - A client integration for connecting to Azure AI Foundry and GitHub Models.
* [GitHub Models](https://www.nuget.org/packages/Aspire.Hosting.GitHub.Models/) - The .NET Aspire GitHub Models integration, provides access to various AI models including OpenAI's GPT models, DeepSeek, Microsoft's Phi models, and other leading AI models, all accessible through GitHub's infrastructure.
* [Ollama](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.Ollama/) - An Aspire hosting integration leveraging the Ollama container with support for downloading a model on startup, with [client](https://www.nuget.org/packages/CommunityToolkit.Aspire.OllamaSharp/) integration.
* [Open AI](https://www.nuget.org/packages/Aspire.Hosting.OpenAI) - Provides extension methods and resource definitions for a .NET Aspire AppHost to configure OpenAI resources and models.

### Authentication and Authorization

* [Keycloak](https://www.nuget.org/packages/Aspire.Hosting.Keycloak) - The .NET Aspire Keycloak integration enables you to connect to existing Keycloak instances or create new instances, with [client](https://www.nuget.org/packages/Aspire.Keycloak.Authentication/) integration.

### AWS

* [Aspire.Hosting.AWS](https://www.nuget.org/packages/Aspire.Hosting.AWS) - Provides extension methods and resources definition for a .NET Aspire AppHost to configure the AWS SDK for .NET and AWS application resources.

### Azure

* [Azure AI OpenAI](https://www.nuget.org/packages/Aspire.Hosting.Azure.CognitiveServices) - Provides extension methods and resource definitions for a .NET Aspire AppHost to configure Azure OpenAI, with [client](https://www.nuget.org/packages/Aspire.Azure.AI.OpenAI) integration.
* [Azure AI Search](https://www.nuget.org/packages/Aspire.Hosting.Azure.Search) - Provides extension methods and resource definitions for a .NET Aspire AppHost to configure Azure AI Search Service, with [client](https://www.nuget.org/packages/Aspire.Azure.Search.Documents) integration.
* [Azure App Configuration](https://www.nuget.org/packages/Aspire.Hosting.Azure.AppConfiguration) - Provides extension methods and resource definitions for a .NET Aspire AppHost to configure Azure App Configuration.
* [Azure Application Insights](https://www.nuget.org/packages/Aspire.Hosting.Azure.ApplicationInsights) - Provides extension methods and resource definitions for a .NET Aspire AppHost to configure Azure Application Insights.
* [Azure Cache for Redis](https://www.nuget.org/packages/Aspire.Hosting.Azure.Redis) - Provides extension methods and resource definitions for a .NET Aspire AppHost to configure Azure Cache for Redis.
* [Azure CosmosDB](https://www.nuget.org/packages/Aspire.Hosting.Azure.CosmosDB) - Provides extension methods and resource definitions for a .NET Aspire AppHost to configure Azure CosmosDB, with [client](https://www.nuget.org/packages/Aspire.Microsoft.Azure.Cosmos) integration.
* [Azure Event Hubs](https://www.nuget.org/packages/Aspire.Hosting.Azure.EventHubs) - Provides extension methods and resource definitions for a .NET Aspire AppHost to configure Azure Event Hubs, with [client](https://www.nuget.org/packages/Aspire.Azure.Messaging.EventHubs) integration.
* [Azure Functions](https://www.nuget.org/packages/Aspire.Hosting.Azure.Functions) - Provides methods to the .NET Aspire hosting model for Azure functions.
* [Azure Key Vault](https://www.nuget.org/packages/Aspire.Hosting.Azure.KeyVault) - Support for Azure Key Vault, a cloud service that provides a secure storage of secrets, such as passwords and database connection strings, with [client](https://www.nuget.org/packages/Aspire.Azure.Security.KeyVault) integration.
* [Azure Operational Insights](https://www.nuget.org/packages/Aspire.Hosting.Azure.OperationalInsights) - Provides extension methods and resource definitions for a .NET Aspire AppHost to configure Azure Log Analytics.
* [Azure PostgreSQL](https://www.nuget.org/packages/Aspire.Hosting.Azure.PostgreSQL) - Provides extension methods and resource definitions for a .NET Aspire AppHost to configure Azure Database for PostgreSQL.
* [Azure Service Bus](https://www.nuget.org/packages/Aspire.Hosting.Azure.ServiceBus) - Provides extension methods and resource definitions for a .NET Aspire AppHost to configure Azure Service Bus, with [client](https://www.nuget.org/packages/Aspire.Azure.Messaging.ServiceBus) integration.
* [Azure SignalR](https://www.nuget.org/packages/Aspire.Hosting.Azure.SignalR) - Provides extension methods and resource definitions for a .NET Aspire AppHost to configure Azure SignalR, with [client](https://www.nuget.org/packages/Microsoft.Azure.SignalR) integration.
* [Azure Storage](https://www.nuget.org/packages/Aspire.Hosting.Azure.Storage) - Provides extension methods and resource definitions for a .NET Aspire AppHost to configure Azure Storage, with [blob client](https://www.nuget.org/packages/Aspire.Azure.Storage.Blobs), [queues client](https://www.nuget.org/packages/Aspire.Azure.Storage.Queues) and [tables client](https://www.nuget.org/packages/Aspire.Azure.Data.Tables) integrations.
* [Azure Web PubSub](https://www.nuget.org/packages/Aspire.Hosting.Azure.WebPubSub) - Provides extension methods and resource definitions for a .NET Aspire AppHost to configure Azure Web PubSub, with [client](https://www.nuget.org/packages/Aspire.Azure.Messaging.WebPubSub) integration.
* [Azure.Dapr.Redis](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.Azure.Dapr.Redis/) - An extension for the Dapr hosting integration for using Dapr with Azure Redis cache.

### Caching

* [Aspire.StackExchange.Redis.DistributedCaching](https://www.nuget.org/packages/Aspire.StackExchange.Redis.DistributedCaching) - Registers an IDistributedCache in the DI container that connects to a Redis server.
* [Aspire.StackExchange.Redis.OutputCaching](https://www.nuget.org/packages/Aspire.StackExchange.Redis.OutputCaching) - Registers an ASP.NET Core Output Caching provider backed by a Redis server.
* [Garnet](https://www.nuget.org/packages/Aspire.Hosting.Garnet/) - An Aspire hosting integration for Garnet.
* [Redis](https://www.nuget.org/packages/Aspire.Hosting.Redis/) - An Aspire hosting integration for Redis, with [client](https://www.nuget.org/packages/Aspire.StackExchange.Redis/) integration.
* [Valkey](https://www.nuget.org/packages/Aspire.Hosting.Valkey/) - An Aspire hosting integration for Valkey.

### Databases

* [Apache Solr](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.Solr/) - An Aspire hosting integration for Apache Solr.
* [Elasticsearch](https://www.nuget.org/packages/Aspire.Hosting.Elasticsearch/) - An Aspire hosting integration for Elasticsearch, with [client](https://www.nuget.org/packages/Aspire.Elastic.Clients.Elasticsearch/) integration.
* [EventStore](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.EventStore/) - An Aspire hosting integration leveraging the EventStore container, with [client](https://www.nuget.org/packages/CommunityToolkit.Aspire.EventStore/) integration.
* [Meilisearch](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.Meilisearch/) - An Aspire hosting integration leveraging the Meilisearch container, with [client](https://www.nuget.org/packages/CommunityToolkit.Aspire.Meilisearch/) integration.
* [Milvus](https://www.nuget.org/packages/Aspire.Hosting.Milvus/) - An Aspire hosting integration for Milvus, with [client](https://www.nuget.org/packages/Aspire.Milvus.Client/) integration.
* [MongoDB](https://www.nuget.org/packages/Aspire.Hosting.MongoDB/) - An Aspire hosting integration for MongoDB, with [client](https://www.nuget.org/packages/Aspire.MongoDB.Driver/) integration.
* [MongoDB extensions](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.MongoDB.Extensions/) - An integration that contains some additional extensions for hosting MongoDB container.
* [MySQL](https://www.nuget.org/packages/Aspire.Hosting.MySql/) - An Aspire hosting integration for MySQL, with [client](https://www.nuget.org/packages/Aspire.MySqlConnector/) integration.
* [MySQL extensions](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.MySql.Extensions/) - An integration that contains some additional extensions for hosting MySQL container.
* [Oracle](https://www.nuget.org/packages/Aspire.Hosting.Oracle/) - An Aspire hosting integration for Oracle.
* [PostgreSQL](https://www.nuget.org/packages/Aspire.Hosting.PostgreSQL/) - An Aspire hosting integration for PostgreSQL, with [client](https://www.nuget.org/packages/Aspire.Npgsql/) integration.
* [PostgreSQL extensions](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.PostgreSQL.Extensions/) - An integration that contains some additional extensions for hosting PostgreSQL container.
* [Qdrant](https://www.nuget.org/packages/Aspire.Hosting.Qdrant/) - An Aspire hosting integration for Qdrant, with [client](https://www.nuget.org/packages/Aspire.Qdrant.Client/) integration.
* [RavenDB](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.RavenDB/) - An Aspire integration leveraging the RavenDB container, with [client](https://www.nuget.org/packages/CommunityToolkit.Aspire.RavenDB.Client/) integration.
* [Redis extensions](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.Redis.Extensions/) - An integration that contains some additional extensions for hosting Redis container.
* [SQL Server](https://www.nuget.org/packages/Aspire.Hosting.SqlServer/) - An Aspire hosting integration for SQL Server, with [client](https://www.nuget.org/packages/Aspire.Microsoft.Data.SqlClient/) integration.
* [SQL Server extensions](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.SqlServer.Extensions/) - An integration that contains some additional extensions for hosting SqlServer container.
* [SQL Server Database Projects](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.SqlDatabaseProjects/) - A hosting integration for the SQL Databases Projects.
* [SQLite](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.Sqlite/) - An Aspire hosting integration to setup a SQLite database with optional SQLite Web as a dev UI, with [client](https://www.nuget.org/packages/CommunityToolkit.Aspire.Microsoft.Data.Sqlite/) integration.
* [SurrealDB](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.SurrealDb/) - An Aspire hosting integration leveraging the SurrealDB container, with [client](https://www.nuget.org/packages/CommunityToolkit.Aspire.SurrealDb/) integration.

### Feature flags

* [Go Feature Flag](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.GoFeatureFlag/) - An Aspire hosting integration leveraging the GoFeatureFlag container, with [client](https://www.nuget.org/packages/CommunityToolkit.Aspire.GoFeatureFlag/) integration.

### Logging

* [Seq](https://www.nuget.org/packages/Aspire.Hosting.Seq/) - An Aspire hosting integration for Seq, with [client](https://www.nuget.org/packages/Aspire.Seq/) integration.

### Mail

* [Papercut SMTP](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.PapercutSmtp) - An Aspire component leveraging Papercut SMTP container.
* [MailPit](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.MailPit/) - An Aspire integration leveraging the MailPit container.

### ORM

* [Aspire.Microsoft.EntityFrameworkCore.Cosmos](https://www.nuget.org/packages/Aspire.Microsoft.EntityFrameworkCore.Cosmos) - Registers EntityFrameworkCore DbContext in the DI container for connecting to Azure Cosmos DB.
* [Aspire.Microsoft.EntityFrameworkCore.SqlServer](https://www.nuget.org/packages/Aspire.Microsoft.EntityFrameworkCore.SqlServer) - Registers EntityFrameworkCore DbContext service for connecting Azure SQL, MS SQL server database.
* [Aspire.Npgsql.EntityFrameworkCore.PostgreSQL](https://www.nuget.org/packages/Aspire.Npgsql.EntityFrameworkCore.PostgreSQL) - Registers EntityFrameworkCore DbContext in the DI container for connecting PostgreSQL database.
* [Aspire.Azure.Npgsql.EntityFrameworkCore.PostgreSQL](https://www.nuget.org/packages/Aspire.Azure.Npgsql.EntityFrameworkCore.PostgreSQL) - Registers EntityFrameworkCore DbContext in the DI container for connecting to PostgreSQL and Azure Database for PostgreSQL.
* [Aspire.Oracle.EntityFrameworkCore](https://www.nuget.org/packages/Aspire.Oracle.EntityFrameworkCore) - Registers EntityFrameworkCore DbContext service for connecting Oracle database.
* [Aspire.Pomelo.EntityFrameworkCore.MySql](https://www.nuget.org/packages/Aspire.Pomelo.EntityFrameworkCore.MySql) - Registers EntityFrameworkCore DbContext in the DI container for connecting MySQL database.
* [Microsoft.EntityFrameworkCore.Sqlite](https://www.nuget.org/packages/CommunityToolkit.Aspire.Microsoft.EntityFrameworkCore.Sqlite/) - An Aspire client integration for the Microsoft.EntityFrameworkCore.Sqlite NuGet package.

### Programming languages

* [Bun](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.Bun) - A hosting integration for the Bun apps.
* [Deno](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.Deno) - A hosting integration for the Deno apps.
* [Golang](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.Golang) - A hosting integration Golang apps.
* [Java](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.Java) - An integration for running Java code in .NET Aspire either using the local JDK or using a container.
* [Node.js](https://www.nuget.org/packages/Aspire.Hosting.NodeJs) - Provides extension methods and resource definitions for a .NET Aspire AppHost to configure a Node.js project.
* [Node.js extensions](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.NodeJS.Extensions) - An integration that contains some additional extensions for running Node.js applications.
* [Python](https://www.nuget.org/packages/Aspire.Hosting.Python) - Support of Python for .NET Aspire.
* [Python extensions](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.Python.Extensions) - An integration that contains some additional extensions for running python applications.
* [Rust](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.Rust) - A hosting integration for the Rust apps.

### Queue and Messaging

* [ActiveMQ](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.ActiveMQ/) - An Aspire hosting integration leveraging the ActiveMQ container.
* [Kafka](https://www.nuget.org/packages/Aspire.Hosting.Kafka/) - An Aspire hosting integration for Apache Kafka, with [client](https://www.nuget.org/packages/Aspire.Confluent.Kafka/) integration.
* [LavinMQ](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.LavinMQ/) - An Aspire hosting integration for LavinMQ.
* [NATS](https://www.nuget.org/packages/Aspire.Hosting.Nats/) - An Aspire hosting integration for the NATS container, with [client](https://www.nuget.org/packages/Aspire.NATS.Net/) integration.
* [RabbitMQ](https://www.nuget.org/packages/Aspire.Hosting.RabbitMQ/) - An Aspire hosting integration for RabbitMQ, with [client](https://www.nuget.org/packages/Aspire.RabbitMQ.Client/) integration.

### Storage

* [MinIO](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.Minio/) - An Aspire hosting integration to setup a MinIO S3 storage, with [client](https://www.nuget.org/packages/CommunityToolkit.Aspire.Minio.Client/) integration.

### Testing

* [Aspire.Hosting.Testing](https://www.nuget.org/packages/Aspire.Hosting.Testing) - Testing support for the .NET Aspire application model.
* [k6](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.k6/) - An Aspire integration leveraging the Grafana k6 container.
* [WireMock](https://www.nuget.org/packages/WireMock.Net.Aspire) - Lightweight Http Mocking Server for .NET, inspired by WireMock.org (from the Java landscape).

### Tools

* [Azure Data API builder](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.Azure.DataApiBuilder/) - A hosting integration for the Azure Data API builder.
* [Dapr](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.Dapr/) - An Aspire hosting integration for Dapr.
* [DevTunnels](https://www.nuget.org/packages/Aspire.Hosting.DevTunnels/) - Provides extension methods and resource definitions for an Aspire AppHost to expose local application endpoints publicly via a secure dev tunnel.
* [Docker](https://www.nuget.org/packages/Aspire.Hosting.Docker/) - Provides publishing extensions to .NET Aspire for Docker Compose.
* [ngrok](https://www.nuget.org/packages/CommunityToolkit.Aspire.Hosting.Ngrok/) - Provides extension methods and resource definitions for a .NET Aspire AppHost to configure a ngrok container.
* [Orleans](https://www.nuget.org/packages/Aspire.Hosting.Orleans) - Provides extension methods and resource definitions for a .NET Aspire AppHost to configure an Orleans cluster.
* [YARP](https://www.nuget.org/packages/Aspire.Hosting.Yarp/) - The .NET Aspire YARP integration enables you to create containerized YARP reverse proxy instances with programmatic configuration or external configuration files.

## Sample Projects

* [aspire-samples](https://github.com/dotnet/aspire-samples) - Official repository of samples for .NET Aspire. 
* [eShop](https://github.com/dotnet/eShop) - An official .NET repository that demonstrates a complete .NET application implementing an eCommerce site.
* [net-aspire-app](https://github.com/leventozz/net-aspire-app) - A basic project with a web frontend, a .NET Core Web API and a Redis cache.
* [PizzaShop](https://github.com/iancooper/PizzaShop) - An example of a messaging pipeline, using Azure Service Bus and Kafka.
* [Aspire AI Chat](https://github.com/davidfowl/aspire-ai-chat-demo) - A full-stack chat sample that combines modern technologies to deliver a ChatGPT-like experience.
* [Url Shortener API](https://github.com/poorna-soysa/url-shortener-app) - This repository showcases a sample API built with .NET 9 that demonstrates the integration of .NET Aspire orchestration. The application utilizes PostgreSQL as database, and Redis for caching.

## Videos

* [Aspire channel](https://www.youtube.com/@aspiredotdev) - The official YouTube channel for .NET Aspire.
* [.NET Aspire for Beginners - Full Series](https://www.youtube.com/watch?v=4ixWtXK7KzY) - A 1h30 video to fully dive into .NET Aspire.
* [.NET Aspire Playlist](https://www.youtube.com/playlist?list=PLdo4fOcmZ0oWTWWbWXqhn2w8NM3sQ_qDz) - A YouTube Playlist that contains dozens of videos regarding .NET Aspire.
* [AspiriFridays](https://www.youtube.com/playlist?list=PLdo4fOcmZ0oUaQPBuCHVscl4OC7E6EMTn) - A YouTube Playlist that contains videos of projects converted to .NET Aspire, on fridays.
* [Custom Tracing with .NET Aspire](https://www.youtube.com/watch?v=vnQg0I5PAUA) - This video talk about adding custom tracing to your application and how it appears on the .NET Aspire dashboard.
* [Custom Metrics with .NET Aspire](https://www.youtube.com/watch?v=mwxJBv0kmcg) - This video talk about adding custom metrics to your application to measure the performance of a feature.
* [Adding Custom Health Checks with .NET Aspire](https://www.youtube.com/watch?v=HuogJghWBks) - This video talk about adding custom health checks and the HealthChecks UI to your application.
* [Adding Custom Commands to the Dashboard](https://www.youtube.com/watch?v=idXn50wKqhY) - This video demonstrates how to add custom commands that allow you to perform tasks directly from the .NET Aspire dashboard.
* [How to run a custom container images in .NET Aspire projects](https://www.youtube.com/watch?v=-6-g5gIWP60) - In this video, Jeff Fritz shows you how to add a container, ANY container, to your application.
* [.NET Aspire - Project Names and Constants](https://www.youtube.com/watch?v=Jt39GzYCRgo) - In this video, Jeff Fritz shows you how to customize how we name projects and reference them throughout the .NET Aspire system.
* [End-to-end integration testing with .NET Aspire](https://www.youtube.com/watch?v=bPIu6PZW41Q) - This video talk how to use the testing features provided by .NET Aspire.
* [Latest Features of .NET Aspire 9.4](https://www.youtube.com/watch?v=9ODsNkpyVDM) - Let's take a look at features introduced in .NET Aspire 9.4.

## Community

* [Discord](https://aka.ms/aspire-discord) - The official Aspire Discord server.
* [aspireify.net](https://aspireify.net/) - A blog regarding .NET Aspire - News, Samples and Tutorials.
