---
title: ポリシーの割り当て
description: アプリケーションまたはサービスプリンシパルにポリシーを割り当てます。
localization_priority: Normal
ms.openlocfilehash: c690aa85d7471aa6ef5da6d1281dfc679e63a09f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337548"
---
# <a name="assign-policy"></a>ポリシーの割り当て

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリケーションまたはサービスプリンシパルに[ポリシー](../resources/policy.md)を割り当てます。

>注: 現時点では、ポリシーの割り当てはトークンの有効期限ポリシーにのみ適用されます。 この種類のポリシーについては、「[ポリシー](../resources/policy.md)」で説明します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求

```http
POST /applications/{id}/policies/$ref
POST /serviceprincipals/{id}/policies/$ref
```

> 注: 要求の "id" は、"appid" プロパティではなく、アプリケーションまたはサービスプリンシパルの "id" プロパティです。

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |
| Content-Type | application/json  | エンティティ本文内のデータの性質です。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、追加するポリシーオブジェクトの JSON 表記を指定します。

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。 失敗した場合、`4xx` エラーが詳細情報とともに返されます。

## <a name="example"></a>例
次の例では、アプリケーションにポリシーを割り当てます。

##### <a name="request"></a>要求
以下は、要求の例です。

```http
POST /applications/{id}/policies/$ref
Content-type: application/json
{
    "@odata.id":"https://graph.microsoft.com/beta/policies/{policyid}"
}
```

##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。

```http
HTTP/1.1 204 No Content
```
