---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

// Code snippets are only available for the latest version. Current version is 6.x

GraphServiceClient graphClient = new GraphServiceClient(requestAdapter);

com.microsoft.graph.beta.security.cases.ediscoverycases.item.searches.item.microsoftgraphsecurityexportresult.ExportResultPostRequestBody exportResultPostRequestBody = new com.microsoft.graph.beta.security.cases.ediscoverycases.item.searches.item.microsoftgraphsecurityexportresult.ExportResultPostRequestBody();
exportResultPostRequestBody.setDisplayName("Export 4");
exportResultPostRequestBody.setExportCriteria(EnumSet.of(com.microsoft.graph.beta.models.security.ExportCriteria.PartiallyIndexed));
exportResultPostRequestBody.setExportLocation(EnumSet.of(com.microsoft.graph.beta.models.security.ExportLocation.ResponsiveLocations, com.microsoft.graph.beta.models.security.ExportLocation.NonresponsiveLocations));
exportResultPostRequestBody.setAdditionalOptions(EnumSet.of(com.microsoft.graph.beta.models.security.AdditionalOptions.TeamsAndYammerConversations, com.microsoft.graph.beta.models.security.AdditionalOptions.CloudAttachments, com.microsoft.graph.beta.models.security.AdditionalOptions.AllDocumentVersions, com.microsoft.graph.beta.models.security.AdditionalOptions.SubfolderContents, com.microsoft.graph.beta.models.security.AdditionalOptions.ListAttachments));
exportResultPostRequestBody.setExportFormat(com.microsoft.graph.beta.models.security.ExportFormat.Eml);
graphClient.security().cases().ediscoveryCases().byEdiscoveryCaseId("{ediscoveryCase-id}").searches().byEdiscoverySearchId("{ediscoverySearch-id}").microsoftGraphSecurityExportResult().post(exportResultPostRequestBody);


```