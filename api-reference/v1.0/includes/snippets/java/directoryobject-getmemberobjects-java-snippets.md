---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean securityEnabledOnly = true;

graphClient.directoryObjects("{object-id}")
	.getMemberObjects(StringGetMemberObjectsParameterSet
		.newBuilder()
		.withSecurityEnabledOnly(securityEnabledOnly)
		.build())
	.buildRequest()
	.post();

```