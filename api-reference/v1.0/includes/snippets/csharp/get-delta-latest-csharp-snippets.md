---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta?token=latest = await graphClient.Me.Drive.Root.Delta?token=latest
	.Request()
	.GetAsync();

```