---
title: ポリシーを更新します。
description: 既存のポリシーのプロパティを更新します。
ms.openlocfilehash: 426476b5545e511fe2da111acb1f47f38f32c96f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073614"
---
# <a name="update-policy"></a>ポリシーを更新します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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
| 名前       | 型 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |
| Content-Type | application/json  | エンティティ本文内のデータの性質です。必須。 |

## <a name="request-body"></a>要求本文
要求の本文には、更新する必要があるパラメーターを使用して JSON オブジェクトを提供します。 次の表は、使用できるパラメーターを示します。

| パラメーター    | 型   |説明|
|:---------------|:--------|:----------|
|definition|String|Stringified[ポリシー](../resources/policy.md)オブジェクトのバージョンです。|
|displayName|String|ポリシーに独自の名前です。|
|isOrganizationDefault|ブール値|既定でこのポリシーを適用するかどうかを指定します。|
|type|String|ポリシーの種類を指定します。 現在、"TokenLifetimePolicy"にする必要があります。|

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。 失敗した場合、`4xx`について、エラーが返されます。

## <a name="example"></a>使用例
次の例では、トークンの有効期間ポリシーの定義を更新し、組織の既定値として設定します。

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
