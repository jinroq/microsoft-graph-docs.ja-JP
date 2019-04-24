---
title: governanceResource を取得する
description: governanceResource オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: be24fb8822101f7a67a5bd60f1fe018cf1a08f6b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463930"
---
# <a name="get-governanceresource"></a>governanceResource を取得する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[governanceResource](../resources/governanceresource.md)オブジェクトのプロパティとリレーションシップを取得します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | PrivilegedAccess AzureResources  |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | PrivilegedAccess AzureResources |

この API は、アクセス許可スコープの他に、リソースに対して少なくとも1つの役割の割り当てを要求する必要があります。

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッド**は**、 `$select`応答`$expand`をカスタマイズするためのおよび[OData クエリパラメーター](/graph/query-parameters)のみをサポートします。

## <a name="request-headers"></a>要求ヘッダー
| 名前      |説明|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。
## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[governanceResource](../resources/governanceresource.md)オブジェクトを返します。

## <a name="example"></a>例
この例では、サブスクリプションの Wingtip Toys-生産 (e5e7d29d-5465-45ac-885f-4716a5ee74b5) の詳細を取得する方法を示します。
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a>要求
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a>応答
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 459

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceResources/$entity",
    "id": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",
    "type": "subscription",
    "displayName": "Wingtip Toys - Prod",
    "status": "Active",
    "registeredDateTime": "2018-04-05T22:30:37.13Z",
    "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceresource-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
