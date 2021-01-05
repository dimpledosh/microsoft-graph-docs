---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveSearchCollectionPage search = graphClient.me().drive()
	.search(DriveItemSearchParameterSet
		.newBuilder()
		.withQ("Contoso Project")
		.build())
	.buildRequest()
	.get();

```