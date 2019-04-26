---
title: アプリケーションまたはサービスプリンシパルに割り当てられているポリシーの一覧
description: アプリケーションまたはサービスプリンシパルに割り当てられているポリシーオブジェクトを取得します。
localization_priority: Normal
ms.openlocfilehash: 24833a42a8b3df2dfde6894cbcdae89a20c6e1cc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332227"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a>アプリケーションまたはサービスプリンシパルに割り当てられているポリシーの一覧

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリケーションまたはサービスプリンシパルに割り当てられている[ポリシー](../resources/policy.md)オブジェクトを取得します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> 注: 要求の "id" は、"appid" プロパティではなく、アプリケーションまたはサービスプリンシパルの "id" プロパティです。

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[ポリシー](../resources/policy.md)オブジェクトを返します。 失敗した場合、`4xx` エラーが詳細情報とともに返されます。

## <a name="example"></a>例
次の例では、アプリケーションに割り当てられているポリシーを取得します。

##### <a name="request"></a>要求
以下は、要求の例です。

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。

```http
HTTP/1.1 200 OK
Cache-Control: private
Content-Type: application/json

{
    "value":[
        {
            "@odata.type":"#microsoft.graph.policy",
            "id":"id-value",
            "alternativeIdentifier":null,
            "definition":["policy-definition"],
            "displayName":"name-value",
            "isOrganizationDefault":boolean-value,
            "keyCredentials":[key-credentials],
            "type":"type-value"
        }
    ]
}
```
