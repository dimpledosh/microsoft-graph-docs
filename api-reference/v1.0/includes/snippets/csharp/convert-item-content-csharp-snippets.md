---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var content?format={format} = await graphClient.Me.Drive.Items["{item-id}"]["content?format={format}"]
	.Request()
	.GetAsync();

```