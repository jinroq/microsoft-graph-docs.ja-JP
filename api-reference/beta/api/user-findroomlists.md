---
title: 'ユーザー: findRoomLists'
description: テナントで定義された部屋の一覧を取得します。
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 55ff393e828d324035050e33cf194cb49d302080
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855735"
---
# <a name="user-findroomlists"></a>ユーザー: findRoomLists

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

テナントで定義された部屋の一覧を取得します。

テナントは、ルーム リストに会議室を整理できます。 各会議室や部屋の一覧は、 [emailAddress](../resources/emailaddress.md)インスタンスによって表されます。
テナント、テナント内の[すべての部屋を取得](user-findrooms.md)を、または[すべての会議室を取得する](user-findrooms.md)特定の会議室の一覧で [すべてのルーム一覧を取得できます。


## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | User.ReadBasic.All、User.Read.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | User.Read.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /me/findRoomLists
GET /users/<id>/findRoomLists

```

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 種類 | 説明 |
|:---------------|:----------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |
| Content-Type  | string  | application/json. Required. |


## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードおよび[emailAddress](../resources/emailaddress.md)コレクション オブジェクト。

テナントのリストが定義されていない場合は、空の配列が返されます。

## <a name="example"></a>例
##### <a name="request"></a>要求

以下は、要求の例です。

<!-- {
  "blockType": "request",
  "name": "user_get_room_lists"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRoomLists
```

##### <a name="response"></a>応答
以下は、応答の例です。 

注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "name": "user_get_room_lists",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAddress",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAddress)",
    "value": [
        {
            "name": "Building 1 Rooms",
            "address": "Building1Rooms@contoso.onmicrosoft.com"
        },
        {
            "name": "Building 2 Rooms",
            "address": "Building2Rooms@contoso.onmicrosoft.com"
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: findRoomLists",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
