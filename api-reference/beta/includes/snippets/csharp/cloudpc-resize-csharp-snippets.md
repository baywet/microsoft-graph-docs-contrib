---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

// Dependencies
using Microsoft.Graph.Beta.DeviceManagement.VirtualEndpoint.CloudPCs.Item.Resize;

var requestBody = new ResizePostRequestBody
{
	TargetServicePlanId = "30d0e128-de93-41dc-89ec-33d84bb662a0",
};

// To initialize your graphClient, see https://learn.microsoft.com/en-us/graph/sdks/create-client?from=snippets&tabs=csharp
await graphClient.DeviceManagement.VirtualEndpoint.CloudPCs["{cloudPC-id}"].Resize.PostAsync(requestBody);


```