# Introduction to Azure Connect for AI

This article series outlines definitive guidance, processes, design patterns, and reference implemenations to enable Integrations to Azure's suite of AI Technologies (Azure OpenAI Service, Microsoft Copilot for Azure, Azure AI Search, ...), using Azure Integration Service in combination with Azure Landing Zones. 

## [What are Azure AI services? - Azure AI services | Microsoft Learn](https://learn.microsoft.com/en-us/azure/ai-services/what-are-ai-services)

todo: comments

## Microsoft Copilot for Azure - AI Companion and Assistant | Microsoft Azure](https://azure.microsoft.com/en-us/products/copilot))

todo: comments



# Integration Design Patterns for AI

Integrating large-scale systems, especially in the context of supporting large language models (LLMs), copilots, and machine learning workloads, requires a robust, secure, and efficient approach. Drawing from established practices, including those found in the "Enterprise Integration Patterns" book, and adapting them to the specific needs of AI architectures, here are 10 design patterns tailored to ensure solid, secure, and timely data integrations.

## Knowledge Retrieveal Pattern

todo: update

## Function Calling Pattern

todo: update

## Thread Context Pattern

todo: update

## Event-Driven Data for AI Pattern

This pattern involves decoupling system components through asynchronous message passing. By using events to trigger data flows organizations can react to changes in real-time, which is crucial for feeding LLMs with the latest data. It supports scalability and resilience, as components can scale independently and failures in one area don't directly impact others which is critical in providing most accurate data in timely manner.

## LLM Content Enricher Pattern

This pattern involves augmenting LLM's with additional data retrieved from other sources. In the context of AI, enriching data in transit can provide models with additional context, improving their accuracy and effectiveness.

## Canonical AI Data Model Pattern

Defining a common AI data format for messages flowing between systems reduces the complexity of data transformations. This is essential for AI and ML systems that integrate with multiple sources, ensuring that data is consistently understood regardless of its origin.



## Gateway Source Data Aggregation Pattern

Combining responses from several services or Systems of Record's (SoR) into a single response reduces the number of round trips while fetching data. This is particularly beneficial in AI systems where a single query may need to pull data from multiple sources to provide a comprehensive answer.
