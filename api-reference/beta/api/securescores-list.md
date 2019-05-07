---
title: secureScores のリスト
description: SecureScores オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: 55a9628d88300a97b62145f22f6fc18fce04b92b
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638810"
---
# <a name="list-securescores"></a>secureScores のリスト

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[SecureScores](../resources/securescores.md)オブジェクトのプロパティとリレーションシップを取得します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  SecurityEvents。 All、SecurityEvents.。   |
|委任 (個人用 Microsoft アカウント) |  サポートされていません。  |
|アプリケーション | SecurityEvents。 All、SecurityEvents.。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a>要求ヘッダー

| 名前      |説明|
|:----------|:----------|
| Authorization  | ベアラー {code}。 必須です。|

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**secureScores**オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求

要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a>応答

応答の例を次に示します。
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection":true,
  "@odata.type": "microsoft.graph.secureScore"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "activeUserCount": 1,
            "createdDateTime": "createdDateTime.value",
            "currentScore": 1,
            "enabledServices": "enabledServices.value",
            "licensedUserCount": 1,
            "maxScore": 1,
            "id": "id.value",
            "azureTenantId": "azureTenantId.value",
            "averageComparativeScores": [
                {
                    "basis": "AllTenants",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value"
                },
                {
                    "basis": "TotalSeats",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value",
                    "seatSizeRangeUpperValue": "seatSizeRangeUpperValue.value",
                    "categoryValue": "categoryValue.value",
                    "seatSizeRangeLowerValue": "seatSizeRangeLowerValue.value"
                },
                {
                    "basis": "IndustryTypes",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value",
                    "categoryValue": "categoryValue.value"
                }
            ],
            "controlScores": [
                {
                    "controlCategory": "controlCategory.value",
                    "controlName": "controlName.value",
                    "description": "description.value",
                    "score": "score.value",
                    "total": "total.value",
                    "count": "count.value"
                }
            ]
        }
    ]
}

```
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/securescores_list-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/securescores_list-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!--
{
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescores-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/securescores-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
