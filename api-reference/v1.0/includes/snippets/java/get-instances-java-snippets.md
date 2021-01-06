---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEventCollectionPage instances = graphClient.me().events("AAMkAGUzYRgWAAA=").instances()
	.buildRequest()
	.get();

```