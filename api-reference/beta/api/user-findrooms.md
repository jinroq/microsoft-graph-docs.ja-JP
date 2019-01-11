---
title: 'ユーザー: findRooms'
description: 'すべての会議室ユーザーのテナントや、特定の場所] ボックスの一覧を取得します。 '
localization_priority: Priority
ms.openlocfilehash: 12ddd4c6956d743322ff86c93c5d445f6966e29a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845417"
---
# <a name="user-findrooms"></a>ユーザー: findRooms

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

すべての会議室ユーザーのテナントや、特定の場所] ボックスの一覧を取得します。 

テナントは、ルーム リストに会議室を整理できます。 各会議室や部屋の一覧は、 [emailAddress](../resources/emailaddress.md)インスタンスによって表されます。 [ルームのすべてのリストを取得](user-findroomlists.md)することができます、テナント、テナント内のすべての部屋を取得または特定の会議室の一覧内のすべての会議室を取得します。 テナントの最初の 100 室取得できます。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | User.ReadBasic.All、User.Read.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | User.Read.All |

## <a name="http-request"></a>HTTP 要求

テナント内のすべての部屋を取得します。

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/<id>/findRooms
```

テナントの特定の会議室の一覧内のすべての会議室を取得します。

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list}')
GET /users/<id>/findRooms(RoomList='{room_list}')
```

## <a name="query-parameters"></a>クエリ パラメーター

| クエリ パラメーター       | 種類 | 説明 |
|:---------------|:----------|:----------|
| RoomList | 文字列 | ルームのリストに関連付けられている SMTP アドレスです。 [EmailAddress](../resources/emailaddress.md)インスタンス、SMTP アドレスが含まれている各部屋の一覧が表示されます。 |

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 種類 | 説明 |
|:---------------|:----------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |
| Content-Type  | string  | application/json. Required. |


## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードおよび[emailAddress](../resources/emailaddress.md)コレクション オブジェクト。


## <a name="example"></a>例

##### <a name="request-1"></a>要求 1

最初の例では、サインインしているユーザーのテナント型で定義されているすべての部屋を取得します。

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms
```

##### <a name="response-1"></a>応答 1
以下は、応答の例です。 

注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "name": "user_get_rooms_in_tenant",
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
            "name": "Conf Room Adams",
            "address": "Adams@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Baker",
            "address": "Baker@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Crystal",
            "address": "Crystal@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Hood",
            "address": "Hood@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Rainier",
            "address": "Rainier@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Stevens",
            "address": "Stevens@contoso.onmicrosoft.com"
        }
    ]
}
```

##### <a name="request-2"></a>要求 2

2 番目の例では、Building2Rooms@contoso.onmicrosoft.com の電子メール アドレスで識別される領域を指定したボックスの一覧で 2 つの部屋を取得します。

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```

##### <a name="response-2"></a>応答 2
以下は、応答の例です。 

注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "name": "user_get_rooms_from_specific_list",
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
            "name": "Conf Room Baker",
            "address": "Baker@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Hood",
            "address": "Hood@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Rainier",
            "address": "Rainier@contoso.onmicrosoft.com"
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: findRooms",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
