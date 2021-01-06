---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Users["97a5a533-833d-494b-b543-c0afe026cb96"].Teamwork.InstalledApps
	.Request()
	.GetAsync();

```