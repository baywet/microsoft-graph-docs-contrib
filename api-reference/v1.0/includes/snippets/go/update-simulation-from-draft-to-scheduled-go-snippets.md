---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


// Code snippets are only available for the latest major version. Current major version is $v1.*

// Dependencies
import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-sdk-go/models"
	  //other-imports
)

requestBody := graphmodels.NewSimulation()
id := "2f5548d1-0dd8-4cc8-9de0-e0d6ec7ea3dc"
requestBody.SetId(&id) 
displayName := "Graph Simulation"
requestBody.SetDisplayName(&displayName) 
durationInDays := int32(7)
requestBody.SetDurationInDays(&durationInDays) 
attackTechnique := graphmodels.CREDENTIALHARVESTING_SIMULATIONATTACKTECHNIQUE 
requestBody.SetAttackTechnique(&attackTechnique) 
attackType := graphmodels.SOCIAL_SIMULATIONATTACKTYPE 
requestBody.SetAttackType(&attackType) 
status := graphmodels.SCHEDULED_SIMULATIONSTATUS 
requestBody.SetStatus(&status) 
includedAccountTarget := graphmodels.NewAddressBookAccountTargetContent()
type := graphmodels.ADDRESSBOOK_ACCOUNTTARGETCONTENTTYPE 
includedAccountTarget.SetType(&type) 
accountTargetEmails := []string {
	"faiza@contoso.com",
}
includedAccountTarget.SetAccountTargetEmails(accountTargetEmails)
requestBody.SetIncludedAccountTarget(includedAccountTarget)
excludedAccountTarget := graphmodels.NewAddressBookAccountTargetContent()
type := graphmodels.ADDRESSBOOK_ACCOUNTTARGETCONTENTTYPE 
excludedAccountTarget.SetType(&type) 
accountTargetEmails := []string {
	"sam@contoso.com",
}
excludedAccountTarget.SetAccountTargetEmails(accountTargetEmails)
requestBody.SetExcludedAccountTarget(excludedAccountTarget)
additionalData := map[string]interface{}{
	"@odata.etag" : "\"0100aa9b-0000-0100-0000-6396fa270000\"", 
	"payload@odata.bind" : "https://graph.microsoft.com/v1.0/security/attacksimulation/payloads/12345678-9abc-def0-123456789a", 
}
requestBody.SetAdditionalData(additionalData)

// To initialize your graphClient, see https://learn.microsoft.com/en-us/graph/sdks/create-client?from=snippets&tabs=go
simulations, err := graphClient.Security().AttackSimulation().Simulations().BySimulationId("simulation-id").Patch(context.Background(), requestBody, nil)


```