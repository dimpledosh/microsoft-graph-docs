---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> groupIdsList = new LinkedList<String>();
groupIdsList.add("groupIds-value");

graphClient.servicePrincipals("{id}")
	.checkMemberGroups(StringCheckMemberGroupsParameterSet
		.newBuilder()
		.withGroupIds(groupIdsList)
		.build())
	.buildRequest()
	.post();

```