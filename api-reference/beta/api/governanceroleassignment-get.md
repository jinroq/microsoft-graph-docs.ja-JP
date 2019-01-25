---
title: GovernanceRoleAssignment を取得します。
description: プロパティと、governanceRoleAssignment の関係を取得します。
localization_priority: Normal
ms.openlocfilehash: f699e1b5332652b2b87f3972d2ae47b06894b2e4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508840"
---
# <a name="get-governanceroleassignment"></a>GovernanceRoleAssignment を取得します。

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

プロパティと、 [governanceRoleAssignment](../resources/governanceroleassignment.md)の関係を取得します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | PrivilegedAccess.ReadWrite.AzureResources  |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | PrivilegedAccess.ReadWrite.AzureResources |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
1. リソース上の[governanceRoleAssignment](../resources/governanceroleassignment.md)を取得します。

    *注: だけでなく、アクセス許可のスコープが必要ですが少なくとも 1 つのロールの割り当てがあるリソースにするには、リクエスター。* 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. 私の[governanceRoleAssignment](../resources/governanceroleassignment.md)を取得します。
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a>省略可能なクエリ パラメーター
このメソッド**以外の[OData クエリ パラメーター](/graph/query-parameters)をサポートして**`$filter`の応答をカスタマイズするためです。

## <a name="request-headers"></a>要求ヘッダー
| 名前      |説明|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。
## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[governanceRoleAssignment](../resources/governanceroleassignment.md)のオブジェクトです。
## <a name="example"></a>例
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
サブスクリプション「Wingtip Toys-商品」で、 [governanceRoleAssignment](../resources/governanceroleassignment.md)を取得します。
##### <a name="request"></a>要求
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a>応答
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 182

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignments/$entity",
    "id": "0ba78f41-ee7a-4227-adb9-1499431b2164",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
    "subjectId": "74487eb5-1630-4fa8-9581-0bb076ea5de3",
    "linkedEligibleRoleAssignmentId": null,
    "externalId": null,
    "startDateTime": "2018-01-22T23:47:19.687Z",
    "endDateTime": "2018-07-21T23:47:02.887Z",
    "memberType": "Direct",
    "assignmentState": "Eligible",
    "status": "Provisioned"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignment-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
