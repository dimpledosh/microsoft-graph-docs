---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Teams["acda442c-78d2-491b-8204-4ef5019c0193"].InstalledApps
	.Request()
	.GetAsync();

```