---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ListItem listItem = graphClient.sites("{site-id}").lists("{list-id}").items("{item-id}")
	.buildRequest()
	.get();

```