---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var instances = await graphClient.Me.Events["AAMkAGUzYRgWAAA="].Instances
	.Request()
	.GetAsync();

```