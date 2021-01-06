---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEventCollectionPage calendarView = graphClient.me().calendar().calendarView()
	.buildRequest()
	.get();

```