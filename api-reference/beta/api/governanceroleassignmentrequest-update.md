---
title: GovernanceRoleAssignmentRequests を更新します。
description: 管理者が意思決定を更新するを有効にする (`AdminApproved`または`AdminDenied`) の状態にある governanceRoleAssignmentRequests の`PendingAdminDecision`。
localization_priority: Normal
ms.openlocfilehash: 3d68e06688922177e2a1a183a9fe4bfc6be6a91d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874936"
---
# <a name="update-governanceroleassignmentrequests"></a>GovernanceRoleAssignmentRequests を更新します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

管理者が意思決定を更新するを有効にする (`AdminApproved`または`AdminDenied`) の状態にある[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)の`PendingAdminDecision`。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

>**注:** この API では、依頼者の少なくとも 1 つある必要があります`Active`管理者の役割の割り当て (`owner`または`user access administrator`) [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)が属しているリソースにします。 

|アクセス許可の種類      | Permissions              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | PrivilegedAccess.ReadWrite.AzureResources  |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | PrivilegedAccess.ReadWrite.AzureResources |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a>要求ヘッダー
| 名前           | 説明|
|:---------------|:----------|
| Authorization  | Bearer {code}|
| Content-type  | application/json|

## <a name="request-body"></a>要求本文

|パラメーター      |型                   |必須 |説明|
|:-------------|:----------------------|:--------|:----------|
|理由        |String                 |✓        |彼の意思決定の管理者によって提供されている理由です。|
|意思決定        |String                 |✓        |役割の割り当て要求の管理者の意思決定します。 として値を更新する必要があります`AdminApproved`または`AdminDenied`。|
|スケジュール      |[governanceSchedule](../resources/governanceschedule.md)|        | 役割の割り当て要求のスケジュールです。 状態の`AdminApproved`、これは必須です。|
|assignmentState      |String|         | 割り当て、および値の状態は、`Eligible`または`Active`。 意思決定の`AdminApproved`、これは必須です。 |
### <a name="response"></a>応答
このメソッドは、要求の状態にあるにのみ適用できます`PendingAdminDecision`。

成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例
##### <a name="request"></a>要求
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
##### <a name="request-body"></a>要求本文
```json
{
  "reason":"approve the request to extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-02-20T07:31:13.451Z",
    "stopDateTime":"2018-05-21T07:31:13.451Z",
    },
  "decision":"AdminApproved",
  "assignmentState": "Eligible"
}
```

##### <a name="response"></a>応答
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UpdateRequest governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
