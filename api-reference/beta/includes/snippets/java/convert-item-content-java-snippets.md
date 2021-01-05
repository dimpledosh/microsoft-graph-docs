---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content content?format={format} = graphClient.drive().items("{item-id}").content?format={format}()
	.buildRequest()
	.get();

```