---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content children?$expand=thumbnails = graphClient.me().drive().items("{item-id}").children?$expand=thumbnails()
	.buildRequest()
	.get();

```