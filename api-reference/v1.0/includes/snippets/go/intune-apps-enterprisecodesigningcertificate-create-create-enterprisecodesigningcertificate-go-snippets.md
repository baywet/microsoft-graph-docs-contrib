---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


// Code snippets are only available for the latest major version. Current major version is $v0.*

// Dependencies
import (
	  "context"
	  "time"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-beta-sdk-go/models"
	  //other-imports
)

requestBody := graphmodels.NewEnterpriseCodeSigningCertificate()
content := []byte("y29udGVudA==")
requestBody.SetContent(&content) 
status := graphmodels.PROVISIONED_CERTIFICATESTATUS 
requestBody.SetStatus(&status) 
subjectName := "Subject Name value"
requestBody.SetSubjectName(&subjectName) 
subject := "Subject value"
requestBody.SetSubject(&subject) 
issuerName := "Issuer Name value"
requestBody.SetIssuerName(&issuerName) 
issuer := "Issuer value"
requestBody.SetIssuer(&issuer) 
expirationDateTime , err := time.Parse(time.RFC3339, "2016-12-31T23:57:57.2481234-08:00")
requestBody.SetExpirationDateTime(&expirationDateTime) 
uploadDateTime , err := time.Parse(time.RFC3339, "2016-12-31T23:58:46.5747426-08:00")
requestBody.SetUploadDateTime(&uploadDateTime) 

// To initialize your graphClient, see https://learn.microsoft.com/en-us/graph/sdks/create-client?from=snippets&tabs=go
enterpriseCodeSigningCertificates, err := graphClient.DeviceAppManagement().EnterpriseCodeSigningCertificates().Post(context.Background(), requestBody, nil)


```