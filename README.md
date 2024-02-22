# Introduction to Azure Connect for AI

This article series outlines definitive guidance, processes, design patterns, and reference implemenations to enable Integrations to Azure's suite of AI Technologies (Azure OpenAI Service, Microsoft Copilot for Azure, Azure AI Search, ...), using Azure Integration Service in combination with Azure Landing Zones. 

## [Azure AI Services](https://learn.microsoft.com/en-us/azure/ai-services/what-are-ai-services)

todo: comments

## [Microsoft Copilot](https://azure.microsoft.com/en-us/products/copilot )

todo: comments



# Integration Design Patterns for AI

Integrating large-scale systems, especially in the context of supporting large language models (LLMs), copilots, and machine learning workloads, requires a robust, secure, and efficient approach. Drawing from established practices, including those found in the "Enterprise Integration Patterns" book, and adapting them to the specific needs of AI architectures, here are 10 design patterns tailored to ensure solid, secure, and timely data integrations.

## Knowledge Retrieveal Pattern

todo: update



![alt text](Images/KnowedgeRetrievealPattern.png "Knowedge Retrieveal Pattern")

## Function Calling Pattern

todo: update



[[IMAGE HERE]]



## Thread Context Pattern

todo: update



[[IMAGE HERE]]



## **AI API Calling Gateway**

Serving as a single entry point for all data requests, an API Gateway can manage authentication, rate limiting, and routing. This pattern is essential for securing access to data services, ensuring that only authorized entities can retrieve or manipulate data, and that systems are not overwhelmed by too many requests.  Enables Citizen AI utilizing the Microsoft Power Platform and this API Calling Gatway to Ingest, Store, Train and Consume data.



[[IMAGE HERE]]

## 

## Event-Driven Data for AI Pattern

This pattern involves decoupling system components through asynchronous message passing. By using events to trigger data flows organizations can react to changes in real-time, which is crucial for feeding LLMs with the latest data. It supports scalability and resilience, as components can scale independently and failures in one area don't directly impact others which is critical in providing most accurate data in timely manner.



[[IMAGE HERE]]



## LLM Content Enricher Pattern

This pattern involves augmenting LLM's with additional data retrieved from other sources. In the context of AI, enriching data in transit can provide models with additional context, improving their accuracy and effectiveness.



[[IMAGE HERE]]



## Canonical AI Data Model Pattern

Defining a common AI data format for messages flowing between systems reduces the complexity of data transformations. This is essential for AI and ML systems that integrate with multiple sources, ensuring that data is consistently understood regardless of its origin.



[[IMAGE HERE]]



## AI Gateway Source Data Aggregation Pattern

Combining responses from several services or Systems of Record's (SoR) into a single response reduces the number of round trips while fetching data. This is particularly beneficial in AI systems where a single query may need to pull data from multiple sources to provide a comprehensive answer.



[[IMAGE HERE]]



## AI Data Lakehouse Pipeline

A modern AI take on the Data Lake and Data Warehouse concepts, integrating a Data Lakehouse as a central repository allows for both structured and unstructured data to be stored, managed, and analyzed efficiently. This is vital for training and refining AI models, providing them access to a wide variety of data in a timely manner.



[[IMAGE HERE]]



## AI API Circuit Breaker

To prevent a failure in one service from cascading through the system, a circuit breaker temporarily halts operations to a particular service when failures reach a threshold. This is critical for maintaining system stability and ensuring that AI services remain available even when certain integrations are experiencing issues.



[[IMAGE HERE]]
