# Introduction to Azure Connect for AI
This article series outlines the definitive guidance, processes, design patterns, and reference implemenations to enable Integrations to Azure's suite of AI Technologies (Azure OpenAI Service, Microsoft Copilot for Azure, Azure AI Search, ...), using Azure Integration Service in combination with Azure Landing Zones. 


## Microsoft Copilot (https://azure.microsoft.com/en-us/products/copilot)
todo: comments

## Azure AI Services (https://learn.microsoft.com/en-us/azure/ai-services/what-are-ai-services)
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
