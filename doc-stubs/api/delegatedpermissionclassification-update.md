---
title: "Update delegatedPermissionClassification"
description: "Update the properties of a delegatedPermissionClassification object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update delegatedPermissionClassification
Namespace: microsoft.graph

Update the properties of a [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /delegatedPermissionClassification
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object.

The following table shows the properties that are required when you create the [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|permissionId|String|**TODO: Add Description**|
|permissionName|String|**TODO: Add Description**|
|classification|permissionClassificationType|**TODO: Add Description**. Possible values are: `low`, `medium`, `high`, `unknownFutureValue`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_delegatedpermissionclassification"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/delegatedPermissionClassification
Content-Type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.delegatedPermissionClassification",
  "permissionId": "String",
  "permissionName": "String",
  "classification": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.delegatedPermissionClassification",
  "id": "53e4de05-de05-53e4-05de-e45305dee453",
  "permissionId": "String",
  "permissionName": "String",
  "classification": "String"
}
```
