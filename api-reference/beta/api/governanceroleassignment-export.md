---
title: エクスポート governanceRoleAssignmentRequests
description: 形式の governanceRoleAssignmentRequests のコレクションを取得する`application/octet-stream`、ブラウザーで .csv ファイルとして解析します。
localization_priority: Normal
ms.openlocfilehash: 82c36f176dfed1a4a848c045ce3274e1152bb953
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522428"
---
# <a name="export-governanceroleassignmentrequests"></a>エクスポート governanceRoleAssignmentRequests

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

形式の[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)のコレクションを取得する`application/octet-stream`、ブラウザーで .csv ファイルとして解析します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | PrivilegedAccess.ReadWrite.AzureResources  |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | PrivilegedAccess.ReadWrite.AzureResources |


## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->リソースの[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)のコレクションをエクスポートします。
    
>**注:** だけでなく、アクセス許可のスコープは、この要求には、リソースに 1 つ以上のロールの割り当てを要求元が必要です。 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

私の[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)のコレクションをエクスポートします。
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a>省略可能なクエリ パラメーター
このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)をサポートします。

## <a name="request-headers"></a>要求ヘッダー
| 名前      |説明|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードとコンテンツの種類の`application/octet-stream`。

## <a name="example"></a>例
この例では、サブスクリプションの Wingtip toys 社の商品で .csv ファイルとしてすべてのロールの割り当てを保存します。 

##### <a name="request"></a>要求
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a>応答
以下は、応答の例です。 
```http
HTTP/1.1 200 OK
Content-Type:application/octet-stream
Content-Length:126

77u/77u/QXNzaWdubWVudCBMZXZlbCxVc2VyIEdyb3VwIE5hbWUsUm9sZSBOYW1lLEVtYWlsLEFzc2lnbm1lbnQgVHlwZSxBc3NpZ25tZW43IFN0YXJ0IFRpbWUgKFVUQyksQXNzaWdubWVudCBFbmQgVGltZdAoVVRDKQ0K

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignment-export.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
