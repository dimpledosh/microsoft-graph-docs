---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IShiftCollectionPage shifts = graphClient.teams("{teamId}").schedule().shifts()
	.buildRequest()
	.get();

```