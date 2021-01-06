---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITimeOffCollectionPage timesOff = graphClient.teams("{teamId}").schedule().timesOff()
	.buildRequest()
	.get();

```