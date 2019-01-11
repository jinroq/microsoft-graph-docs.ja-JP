---
title: アプリケーションとサービス ・ プリンシパルに割り当てられている特定のポリシーを一覧表示します。
description: 割り当てられている指定されたポリシーを使用して、アプリケーションとサービスのプリンシパル オブジェクトを取得します。
localization_priority: Normal
ms.openlocfilehash: 21a5a9ba4260e306553f53866657a482d814b5f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875608"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a>アプリケーションとサービス ・ プリンシパルに割り当てられている特定のポリシーを一覧表示します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

割り当てられている指定されたポリシーを使用して、[アプリケーション](../resources/application.md)と[サービス ・ プリンシパル](../resources/serviceprincipal.md)オブジェクトを取得します。

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
| 名前       | 種類 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

かどうかは成功すると、このメソッドを返します`200 OK`応答本体に応答コードおよび[アプリケーション](../resources/application.md)と[サービス ・ プリンシパル](../resources/serviceprincipal.md)のオブジェクトです。 失敗した場合、`4xx`について、エラーが返されます。

## <a name="example"></a>例
次の使用例は、割り当てられている特定のポリシーを使用して、アプリケーションとサービス ・ プリンシパルを取得します。

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
