---
title: ポリシーを作成します。
description: 表示名、ポリシーの種類、およびポリシーの説明を指定することにより、新しいポリシー オブジェクトを作成します。
ms.openlocfilehash: fca6201d7afa6a78f15da0d37fb611e4114783e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073613"
---
# <a name="create-policy"></a>ポリシーを作成します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

表示名、ポリシーの種類、およびポリシーの説明を指定することにより、新しい[ポリシー](../resources/policy.md)オブジェクトを作成します。

>注: ポリシーの詳細が保存される前に検証されます。 検証が合格しなかった場合、400 正しくない要求が返されます。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求

```http
POST /policies
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |
| Content-Type | application/json  | エンティティ本文内のデータの性質です。必須。 |

## <a name="request-body"></a>要求本文
要求の本文には、[ポリシー](../resources/policy.md)オブジェクトの JSON 表現を提供します。

ポリシーを作成するときに必要なプロパティを次の表に示します。

| パラメーター    | 型   |説明|
|:---------------|:--------|:----------|
|definition|String|[ポリシー](../resources/policy.md)オブジェクトの文字列形式。|
|displayName|String|ポリシーに独自の名前です。|
|type|String|ポリシーの種類を指定します。 現在、"TokenLifetimePolicy"にする必要があります。|

## <a name="response"></a>応答

かどうかは成功すると、このメソッドを返します`201 Created`応答本体に応答コードおよび[ポリシー](../resources/policy.md)のオブジェクトです。 失敗した場合、`4xx`について、エラーが返されます。  

## <a name="example"></a>使用例
次の使用例は、新しいトークンの有効期間ポリシーを作成します。 文字列定義のパラメーターは二重引用符をエスケープしたことを確認します。

##### <a name="request"></a>要求
以下は、要求の例です。

```http
POST https://graph.microsoft.com/beta/policies
Content-Type: application/json

{
  "displayName":"CustomTokenLifetimePolicy",
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "type":"TokenLifetimePolicy"
}
```

##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#policies/$entity",
  "id":"id-value",
  "alternativeIdentifier":null,
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "displayName":"name-value",
  "isOrganizationDefault":false,
  "keyCredentials",
  "type":"TokenLifetimePolicy"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
