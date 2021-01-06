---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOnlineMeetingCollectionPage onlineMeetings = graphClient.communications().onlineMeetings()
	.buildRequest()
	.get();

```