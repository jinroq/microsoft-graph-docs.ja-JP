---
title: ポリシーの更新
description: 既存のポリシーのプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: 53b7af8966c932598328e8b78e76022ca6db9c8a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337399"
---
# <a name="update-policy"></a>ポリシーの更新

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

既存の[ポリシー](../resources/policy.md)のプロパティを更新します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求

```http
PATCH /policies/{id}
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 種類 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |
| Content-Type | application/json  | エンティティ本文内のデータの性質です。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、更新する必要があるパラメーターを含む JSON オブジェクトを指定します。 次の表に、使用可能なパラメーターを示します。

| パラメーター    | 型   |説明|
|:---------------|:--------|:----------|
|definition|String|文字列バージョンの[ポリシー](../resources/policy.md)オブジェクト。|
|displayName|文字列|ポリシーのカスタム名。|
|is組織既定|Boolean|このポリシーを既定で適用するかどうかを指定します。|
|type|String|ポリシーの種類を指定します。 現在、"TokenLifetimePolicy" である必要があります。|

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。 失敗した場合、`4xx` エラーが詳細情報とともに返されます。

## <a name="example"></a>例
次の例では、トークン有効期限ポリシーの定義を更新し、それを組織の既定値として設定します。

##### <a name="request"></a>要求
以下は、要求の例です。

```http
PATCH https://graph.microsoft.com/beta/policies/{id}
Content-Type: application/json
{
    "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
    "isOrganizationDefault":true
}
```

##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。

```http
HTTP/1.1 204 No Content
```
