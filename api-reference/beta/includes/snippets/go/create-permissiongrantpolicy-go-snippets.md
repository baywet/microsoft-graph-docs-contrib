---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


// Code snippets are only available for the latest major version. Current major version is $v0.*

// Dependencies
import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-beta-sdk-go/models"
	  //other-imports
)

requestBody := graphmodels.NewPermissionGrantPolicy()
id := "my-custom-consent-policy"
requestBody.SetId(&id) 
displayName := "Custom application consent policy"
requestBody.SetDisplayName(&displayName) 
description := "A custom permission grant policy to customize conditions for granting consent."
requestBody.SetDescription(&description) 

// To initialize your graphClient, see https://learn.microsoft.com/en-us/graph/sdks/create-client?from=snippets&tabs=go
permissionGrantPolicies, err := graphClient.Policies().PermissionGrantPolicies().Post(context.Background(), requestBody, nil)


```