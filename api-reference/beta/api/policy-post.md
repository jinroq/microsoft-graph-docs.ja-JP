---
title: ポリシーの作成
description: 表示名、ポリシーの種類、およびポリシーの説明を指定して、新しいポリシーオブジェクトを作成します。
localization_priority: Normal
ms.openlocfilehash: 4521f6fb032f936aec27cc5cac47d27e62bd2a3a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332200"
---
# <a name="create-policy"></a>ポリシーの作成

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示名、ポリシーの種類、およびポリシーの説明を指定して、新しい[ポリシー](../resources/policy.md)オブジェクトを作成します。

>注: ポリシーの詳細は、保存される前に検証されます。 検証に合格しない場合は、400不良要求が返されます。

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
| 名前       | 種類 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |
| Content-Type | application/json  | エンティティ本文内のデータの性質です。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、 [policy](../resources/policy.md)オブジェクトの JSON 表記を指定します。

次の表に、ポリシーの作成時に必要なプロパティを示します。

| パラメーター    | 型   |説明|
|:---------------|:--------|:----------|
|definition|String|[ポリシー](../resources/policy.md)オブジェクトの文字列バージョン。|
|displayName|文字列|ポリシーのカスタム名。|
|type|String|ポリシーの種類を指定します。 現在、"TokenLifetimePolicy" である必要があります。|

## <a name="response"></a>応答

成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[ポリシー](../resources/policy.md)オブジェクトを返します。 失敗した場合、`4xx` エラーが詳細情報とともに返されます。  

## <a name="example"></a>例
次の例では、新しいトークンの有効期間ポリシーを作成します。 文字列定義パラメーターには二重引用符がエスケープされていることに注意してください。

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
<!--
{
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
