---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserReminderViewCollectionPage reminderView = graphClient.me()
	.reminderView(ReminderReminderViewParameterSet
		.newBuilder()
		.withStartDateTime("2017-06-05T10:00:00.0000000")
		.withEndDateTime("2017-06-11T11:00:00.0000000")
		.build())
	.buildRequest()
	.get();

```