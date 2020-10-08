---
title: "Get onSignupStart"
description: "Read the properties and relationships of an authenticationAction object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get onSignupStart
Namespace: microsoft.graph

Read the properties and relationships of an [authenticationAction](../resources/authenticationaction.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|Policy.ReadWrite.ApplicationConfiguration, Policy.Read.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|Policy.ReadWrite.ApplicationConfiguration, Policy.Read.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/events/onSignupStart/{id}
```

## Optional query parameters

This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [authenticationAction](../resources/authenticationaction.md) object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "get_authenticationaction"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
```

### Response

**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationAction"
}
-->

``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.invokeUserFlowAction",
    "id": "2adb5c12-5c12-2adb-125c-db2a125cdb2a",
    "priority": "101",
    "sourceFilter": {
        "includeApplications": [
            "3dfff01b-0afb-4a07-967f-d1ccbd81102a"
        ]
     }
  }
}
```