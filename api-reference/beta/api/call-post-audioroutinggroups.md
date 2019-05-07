---
title: 音声ルーティング グループを作成する
description: 新しい**audioRoutingGroup**を作成します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a8bd4e0c1e3e78152df9631b2fd4ed06f6df7c69
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635877"
---
# <a name="create-audio-routing-group"></a>音声ルーティング グループを作成する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

新しい**audioRoutingGroup**を作成します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
|:---------------------------------------|:--------------------------------------------|
| 委任 (職場または学校のアカウント)     | サポートされていません。                               |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。                               |
| アプリケーション                            | JoinGroupCalls を呼び出します。すべて、InitiateGroupCalls を呼び出します。 |

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
要求本文で、 [audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトの JSON 表記を指定します。

## <a name="response"></a>応答
成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトを返します。

## <a name="examples"></a>例

### <a name="example-1-one-to-one-audio-routing-group"></a>例 1: 1 対1の音声ルーティンググループ

##### <a name="request"></a>要求
次の例は要求を示しています。

<!-- {
  "blockType": "request",
  "name": "create-audioRoutingGroup-from-call"
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

要求本文で、 [audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトの JSON 表記を指定します。

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
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/create-audioRoutingGroup-from-call-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-audioRoutingGroup-from-call-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
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
  "name": "create-audioRoutingGroup-from-call",
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

要求本文で、 [audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトの JSON 表記を指定します。

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
<!--
{
  "type": "#page.annotation",
  "description": "Create audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-post-audioroutinggroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-post-audioroutinggroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
