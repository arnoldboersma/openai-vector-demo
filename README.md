# Openai vector demo

This repository contains a .NET console application that demonstrates how to generate text embeddings using Azure OpenAI, insert those embeddings into vector fields in Azure Cognitive Search, and issue vector queries. Queries include vector searches with metadata filtering and hybrid (text + vectors) search. The code uses Azure OpenAI to generate embeddings for titleVector and contentVector fields. You'll need access to Azure OpenAI to run this demo.

## Add secrets

```bash
dotnet user-secrets set AZURE_SEARCH_SERVICE_ENDPOINT https://x.search.windows.net
dotnet user-secrets set AZURE_SEARCH_INDEX_NAME cog-search-demo-arnold
dotnet user-secrets set AZURE_SEARCH_ADMIN_KEY KEY
dotnet user-secrets set AZURE_OPENAI_API_KEY KEY
dotnet user-secrets set AZURE_OPENAI_ENDPOINT https://NAME.openai.azure.com/
dotnet user-secrets set AZURE_OPENAI_EMBEDDING_DEPLOYED_MODEL text-embedding-ada-002
```
