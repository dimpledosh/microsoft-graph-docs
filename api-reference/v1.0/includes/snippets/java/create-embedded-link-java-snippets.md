---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "embed";

graphClient.me().drive().items("{item-id}")
	.createLink(PermissionCreateLinkParameterSet
		.newBuilder()
		.withType(type)
		.withScope(null)
		.withExpirationDateTime(null)
		.withPassword(null)
		.withMessage(null)
		.build())
	.buildRequest()
	.post();

```