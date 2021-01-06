---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content thumbnails?select=c300x400_Crop = graphClient.me().drive().items("{item-id}").thumbnails?select=c300x400_Crop()
	.buildRequest()
	.get();

```