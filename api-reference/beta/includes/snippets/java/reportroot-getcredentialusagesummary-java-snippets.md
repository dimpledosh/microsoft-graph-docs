---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReportRootGetCredentialUsageSummaryCollectionPage getCredentialUsageSummary = graphClient.reports()
	.getCredentialUsageSummary(CredentialUsageSummaryGetCredentialUsageSummaryParameterSet
		.newBuilder()
		.withPeriod("D30")
		.build())
	.buildRequest()
	.filter("feature eq 'registration'")
	.get();

```