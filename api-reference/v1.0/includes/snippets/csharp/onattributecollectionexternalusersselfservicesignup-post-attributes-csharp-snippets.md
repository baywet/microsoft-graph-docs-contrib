---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

// Dependencies
using Microsoft.Graph.Models;

var requestBody = new ReferenceCreate
{
	OdataId = "https://graph.microsoft.com/v1.0/identity/userFlowAttributes/city",
};

// To initialize your graphClient, see https://learn.microsoft.com/en-us/graph/sdks/create-client?from=snippets&tabs=csharp
await graphClient.Identity.AuthenticationEventsFlows["{authenticationEventsFlow-id}"].GraphExternalUsersSelfServiceSignUpEventsFlow.OnAttributeCollection.GraphOnAttributeCollectionExternalUsersSelfServiceSignUp.Attributes.Ref.PostAsync(requestBody);


```