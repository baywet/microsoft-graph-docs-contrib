---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

// Dependencies
using Microsoft.Graph.Models;

var requestBody = new ExternalUsersSelfServiceSignUpEventsFlow
{
	OdataType = "#microsoft.graph.externalUsersSelfServiceSignUpEventsFlow",
	OnAttributeCollection = new OnAttributeCollectionExternalUsersSelfServiceSignUp
	{
		OdataType = "#microsoft.graph.onAttributeCollectionExternalUsersSelfServiceSignUp",
		AttributeCollectionPage = new AuthenticationAttributeCollectionPage
		{
			Views = new List<AuthenticationAttributeCollectionPageViewConfiguration>
			{
				new AuthenticationAttributeCollectionPageViewConfiguration
				{
					Title = null,
					Description = null,
					Inputs = new List<AuthenticationAttributeCollectionInputConfiguration>
					{
						new AuthenticationAttributeCollectionInputConfiguration
						{
							Attribute = "email",
							Label = "Email Address",
							InputType = AuthenticationAttributeCollectionInputType.Text,
							DefaultValue = null,
							Hidden = true,
							Editable = false,
							WriteToDirectory = true,
							Required = true,
							ValidationRegEx = "^[a-zA-Z0-9.!#$%&amp;&#8217;'*+/=?^_`{|}~-]+@[a-zA-Z0-9-]+(?:.[a-zA-Z0-9-]+)*$",
							Options = new List<AuthenticationAttributeCollectionOptionConfiguration>
							{
							},
						},
						new AuthenticationAttributeCollectionInputConfiguration
						{
							Attribute = "displayName",
							Label = "Display Name",
							InputType = AuthenticationAttributeCollectionInputType.Text,
							DefaultValue = null,
							Hidden = false,
							Editable = true,
							WriteToDirectory = true,
							Required = false,
							ValidationRegEx = "^[a-zA-Z_][0-9a-zA-Z_ ]*[0-9a-zA-Z_]+$",
							Options = new List<AuthenticationAttributeCollectionOptionConfiguration>
							{
							},
						},
						new AuthenticationAttributeCollectionInputConfiguration
						{
							Attribute = "extension_6ea3bc85aec24b1c92ff4a117afb6621_Favoritecolor",
							Label = "Favorite color",
							InputType = AuthenticationAttributeCollectionInputType.Text,
							DefaultValue = null,
							Hidden = false,
							Editable = true,
							WriteToDirectory = true,
							Required = false,
							ValidationRegEx = "^.*",
							Options = new List<AuthenticationAttributeCollectionOptionConfiguration>
							{
							},
						},
					},
				},
			},
		},
	},
};

// To initialize your graphClient, see https://learn.microsoft.com/en-us/graph/sdks/create-client?from=snippets&tabs=csharp
var result = await graphClient.Identity.AuthenticationEventsFlows["{authenticationEventsFlow-id}"].PatchAsync(requestBody);


```