---
title: 特定のポリシーが割り当てられたアプリケーションとサービスプリンシパルを一覧表示する
description: 指定したポリシーが割り当てられているアプリケーションおよびサービスプリンシパルオブジェクトを取得します。
localization_priority: Normal
ms.openlocfilehash: d7449428216a2e68d9ab8bb8399ca0e8dc4b72fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538754"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a>特定のポリシーが割り当てられたアプリケーションとサービスプリンシパルを一覧表示する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定したポリシーが割り当てられている[アプリケーション](../resources/application.md)および[サービスプリンシパル](../resources/serviceprincipal.md)オブジェクトを取得します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
```http
GET /policies/{id}/appliesTo
```

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[アプリケーション](../resources/application.md)と[サービスプリンシパル](../resources/serviceprincipal.md)オブジェクトを返します。 失敗した場合、`4xx` エラーが詳細情報とともに返されます。

## <a name="example"></a>例
次の例では、特定のポリシーが割り当てられたアプリケーションとサービスプリンシパルを取得します。

##### <a name="request"></a>要求
以下は、要求の例です。

```http
GET https://graph.microsoft.com/beta/policies/{id}/appliesTo
```

##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value":[
        {
            "@odata.type"="#microsoft.graph.application",
            "appId":"appId-value",
            "displayName":"displayName-value",
            "errorUrl":"errorUrl-value",
            "groupMembershipClaims":"groupMembershipClaims-value",
            "homepage":"homepage-value",
            "id":"id-value",
            "keyCredentials":[key-credentials],
            "logoutUrl":"logoutUrl-value",
            "replyUrls":["replyUrls-value"]
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-list-appliesto.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
