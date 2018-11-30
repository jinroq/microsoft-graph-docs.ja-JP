---
title: オーディオのルーティング グループを作成します。
description: 新しい**audioRoutingGroup**を作成します。
ms.openlocfilehash: 9e42fb085887cee22ccc8eac0997adf0464e0d55
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068290"
---
# <a name="create-audio-routing-group"></a>オーディオのルーティング グループを作成します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

新しい**audioRoutingGroup**を作成します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
|:---------------------------------------|:--------------------------------------------|
| 委任 (職場または学校のアカウント)     | サポートされていません。                               |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。                               |
| アプリケーション     | Calls.JoinGroupCallsasGuest.All、Calls.JoinGroupCalls.All、Calls.InitiateGroupCalls.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="request-headers"></a>要求ヘッダー
| 名前          | 説明               |
|:--------------|:--------------------------|
| Authorization | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
要求の本文には、 [audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトの JSON 表現を指定します。

## <a name="response"></a>応答
かどうかは成功すると、このメソッドを返します`200 OK`、応答の本体で応答コードと[audioRoutingGroup](../resources/audioroutinggroup.md)のオブジェクトです。

## <a name="examples"></a>例

### <a name="example-1-one-to-one-audio-routing-group"></a>例 1: 1 対 1 のオーディオ ルーティング グループ

##### <a name="request"></a>要求
次の例は要求を示しています。

<!-- {
  "blockType": "request",
  "name": "create_audioRoutingGroup_from_call"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
Content-Type: application/json
Content-Length: 233

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f"
  ]
}
```

要求の本文には、 [audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトの JSON 表現を指定します。

##### <a name="response"></a>応答

> **注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f"
  ]
}
```
### <a name="example-2-multicast-audioroutinggroup"></a>例 2: マルチキャスト audioRoutingGroup

##### <a name="request"></a>要求
次の例は要求を示しています。

```http
POST https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
Content-Type: application/json
Content-Length: 233
```

<!-- {
  "blockType": "example",
  "name": "create_audioRoutingGroup_from_call",
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->

```json
{
  "id": "multicast",
  "routingMode": "multicast",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```

要求の本文には、 [audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトの JSON 表現を指定します。

##### <a name="response"></a>応答

> **注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233
```
<!-- {
  "blockType": "example",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->

```json
{
  "id": "multicast",
  "routingMode": "multicast",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
