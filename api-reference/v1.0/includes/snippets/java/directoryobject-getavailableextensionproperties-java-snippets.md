---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean isSyncedFromOnPremises = false;

graphClient.directoryObjects()
	.getAvailableExtensionProperties(ExtensionPropertyGetAvailableExtensionPropertiesParameterSet
		.newBuilder()
		.withIsSyncedFromOnPremises(isSyncedFromOnPremises)
		.build())
	.buildRequest()
	.post();

```