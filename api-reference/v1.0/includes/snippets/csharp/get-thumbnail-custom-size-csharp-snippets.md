---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var thumbnails?select=c300x400_Crop = await graphClient.Me.Drive.Items["{item-id}"].Thumbnails?select=c300x400_Crop
	.Request()
	.GetAsync();

```