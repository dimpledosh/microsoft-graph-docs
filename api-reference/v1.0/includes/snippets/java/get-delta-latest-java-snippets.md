---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content delta?token=latest = graphClient.me().drive().root().delta?token=latest()
	.buildRequest()
	.get();

```