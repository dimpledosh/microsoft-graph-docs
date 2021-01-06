---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeView workbookRangeView = graphClient.me().drive().root().workbook().worksheets("{id}")
	.range(WorkbookWorksheetRangeParameterSet
		.newBuilder()
		.withAddress("A1:Z10")
		.build())
	.visibleView()
	.buildRequest()
	.get();

```