---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReportRootGetRelyingPartyDetailedSummaryCollectionPage getRelyingPartyDetailedSummary = graphClient.reports()
	.getRelyingPartyDetailedSummary(RelyingPartyDetailedSummaryGetRelyingPartyDetailedSummaryParameterSet
		.newBuilder()
		.withPeriod("period_value")
		.build())
	.buildRequest()
	.get();

```