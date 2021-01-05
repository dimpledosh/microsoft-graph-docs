---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children?$expand=thumbnails = await graphClient.Me.Drive.Items["{item-id}"].Children?$expand=thumbnails
	.Request()
	.GetAsync();

```