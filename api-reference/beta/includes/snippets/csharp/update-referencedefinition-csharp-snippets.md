---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

// Dependencies
using Microsoft.Graph.Beta.Models.IndustryData;

var requestBody = new ReferenceDefinition
{
	OdataType = "#microsoft.graph.industryData.referenceDefinition",
	DisplayName = "Updated Test Grade Name",
};

// To initialize your graphClient, see https://learn.microsoft.com/en-us/graph/sdks/create-client?from=snippets&tabs=csharp
var result = await graphClient.External.IndustryData.ReferenceDefinitions["{referenceDefinition-id}"].PatchAsync(requestBody);


```