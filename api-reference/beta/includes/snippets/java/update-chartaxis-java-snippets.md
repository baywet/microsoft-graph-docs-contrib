---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

// Code snippets are only available for the latest version. Current version is 6.x

GraphServiceClient graphClient = new GraphServiceClient(requestAdapter);

WorkbookChartAxis workbookChartAxis = new WorkbookChartAxis();
MajorUnit majorUnit = new MajorUnit();
workbookChartAxis.setMajorUnit(majorUnit);
Maximum maximum = new Maximum();
workbookChartAxis.setMaximum(maximum);
Minimum minimum = new Minimum();
workbookChartAxis.setMinimum(minimum);
WorkbookChartAxis result = graphClient.drives().byDriveId("{drive-id}").items().byDriveItemId("{driveItem-id}").workbook().worksheets().byWorkbookWorksheetId("{workbookWorksheet-id}").charts().byWorkbookChartId("{workbookChart-id}").axes().valueAxis().patch(workbookChartAxis);


```