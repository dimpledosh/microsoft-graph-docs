---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookUserSupportedTimeZonesCollectionPage supportedTimeZones = graphClient.me().outlook()
	.supportedTimeZones(TimeZoneInformationSupportedTimeZonesParameterSet
		.newBuilder()
		.withTimeZoneStandard(microsoft.graph.timeZoneStandard'Iana')
		.build())
	.buildRequest()
	.get();

```