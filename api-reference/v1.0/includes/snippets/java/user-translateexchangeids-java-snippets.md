---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> inputIdsList = new LinkedList<String>();
inputIdsList.add("{rest-formatted-id-1}");
inputIdsList.add("{rest-formatted-id-2}");

ExchangeIdFormat sourceIdType = ExchangeIdFormat.REST_ID;

ExchangeIdFormat targetIdType = ExchangeIdFormat.REST_IMMUTABLE_ENTRY_ID;

graphClient.me()
	.translateExchangeIds(ConvertIdResultTranslateExchangeIdsParameterSet
		.newBuilder()
		.withInputIds(inputIdsList)
		.withTargetIdType(targetIdType)
		.withSourceIdType(sourceIdType)
		.build())
	.buildRequest()
	.post();

```