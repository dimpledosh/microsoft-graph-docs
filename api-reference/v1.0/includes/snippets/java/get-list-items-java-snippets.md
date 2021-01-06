---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IListItemCollectionPage items = graphClient.sites("{site-id}").lists("{list-id}").items()
	.buildRequest()
	.get();

```