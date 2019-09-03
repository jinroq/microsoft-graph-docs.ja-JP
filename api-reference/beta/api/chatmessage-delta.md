---
title: 'chatMessages: デルタ'
description: チームのチャネルに含まれるメッセージの一覧を取得します (返信は含めず)。 デルタ クエリを使用すると、チャネルで新しいメッセージや更新されたメッセージを取得できます。
localization_priority: Priority
doc_type: apiPageType
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 38abe022c745219cb8fe3ccd0a717b257ab7c66f
ms.sourcegitcommit: cca4f96414aededa03bb45e07e19bb20b7327563
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/30/2019
ms.locfileid: "36677209"
---
# <a name="chatmessages-delta"></a>chatMessages: デルタ

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チーム](../resources/team.md)の[チャネル](../resources/channel.md)で[メッセージ](../resources/chatmessage.md)の一覧を取得します (返信は含めず)。 デルタ クエリを使用すると、チャネルで新しいメッセージや更新されたメッセージを取得できます。

デルタ クエリでは、指定したチャネル内のすべてのメッセージを取得する完全な同期と、最後の同期以降にチャネルで変更されたメッセージを取得する増分同期の両方がサポートされています。 通常は、最初の完全同期を実行して、その後、そのカレンダー ビューへの増分の変更を定期的に取得します。

メッセージの返信を取得するには、[メッセージの返信一覧](channel-get-messagereply.md)の操作または[メッセージの返信取得](channel-list-messagereplies.md)の操作を使用します。

デルタ関数を使用した GET 要求は、次のいずれかを返します。

- `nextLink` (**デルタ**関数の呼び出しと `skipToken` を使用した URL を含みます)、または
- `deltaLink` (**デルタ**関数の呼び出しと `deltaToken` を使用した URL を含みます)。

状態トークンは、クライアントに対して完全に不透明です。 変更追跡のラウンドを続行する手順は、最後の GET 要求から返された `nextLink` または `deltaLink` の URL を、その同じカレンダー ビューの次のデルタ関数呼び出しにコピーして適用するだけです。 応答で返される `deltaLink` は、変更追跡の現在のラウンドが完了したことを示します。 `deltaLink` URL を保存して、次のラウンドを開始する際に使用することができます。

詳細については、[デルタ クエリ](/graph/delta-query-overview.md)に関するドキュメントを参照してください。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference.md)」を参照してください。

|アクセス許可の種類                        |アクセス許可 (特権の小さいものから大きいものへ)  |
|---------------------------------------|---------------------------------------------|
|委任 (職場または学校のアカウント)     |Group.Read.All、Group.ReadWrite.All          |
|委任 (個人用 Microsoft アカウント) |サポート対象外                                |
|Application                            |Group.Read.All、Group.ReadWrite.All          |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/delta
```

## <a name="query-parameters"></a>クエリ パラメーター

チャネル メッセージの変更を追跡すると、1 つ以上の**デルタ**関数呼び出しのラウンドが発生します。 任意のクエリ パラメーター (`$deltatoken` と`$skiptoken`以外) を使用する場合は、最初の**デルタ**要求でこれを指定する必要があります。 Microsoft Graph は、応答で提供される `nextLink` または `deltaLink` の URL のトークン部分に指定したパラメーターを自動的にエンコードします。

すべてのクエリ パラメーターを最初に 1 回指定しておくだけで済みます。

その後の要求では、以前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みのパラメーターがこの URL に既に含まれているためです。

| クエリ パラメーター      | 種類   |説明|
|:---------------|:--------|:----------|
| `$deltatoken` | string | 前回の**デルタ**関数呼び出しの `deltaLink` URL で返された[状態トークン](/graph/delta-query-overview)で、そのラウンドの変更追跡が完了したことを示します。 このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。|
| `$skiptoken` | string | 以前の**デルタ**関数呼び出しの `nextLink` URL 内で返された[状態トークン](/graph/delta-query-overview)で、同じカレンダー ビュー内に追跡する必要がある変更が他にもあることを示しています。 |

### <a name="optional-odata-query-parameters"></a>オプションの OData クエリ パラメーター

次の [OData クエリ パラメーター](/graph/query-parameters)はこの API でサポートされています。
- `$top`は、1 回の呼び出しで取得するメッセージの最大数を表します。 上限は **50** です。
- `$skip`は、一覧の先頭でスキップするメッセージの数を表します。
- `$filter` により、特定の条件を満たすメッセージを返すことが可能になります。 フィルター処理がサポートされているプロパティは `lastModifiedDateTime` のみで、サポートされている演算子は **gt** と **ge** のみです。 たとえば、`../messages/delta?$filter=lastModifiedDateTime ge 2019-02-27T07:13:28.000z` は、指定した日時以降に作成または変更されたすべてのメッセージを取得します。

## <a name="request-headers"></a>要求ヘッダー
| ヘッダー        | 値                     |
|---------------|---------------------------|
| Authorization | ベアラー {トークン}。必須。 |
| Content-Type  | application/json          |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

このメソッドは、成功すると `200 OK` 応答コードと [chatMessage](https://docs.microsoft.com/ja-JP/graph/api/resources/chatmessage?view=graph-rest-beta) オブジェクトのコレクションを応答本文で返します。 応答には `nextLink` URL または `deltaLink` URLも含まれます。

## <a name="examples"></a>例

### <a name="example-1-initial-synchronization"></a>例 1: 初期同期

次の例では、特定のチャネル内のメッセージを同期するための、3 つの一連の要求を示しています。 チャネルにはメッセージが 5 つあります。

- 手順 1: [最初の要求のサンプル](#initial-request)と[応答](#initial-request-response)。
- 手順 2: [2 番目の要求のサンプル](#second-request)と[応答](#second-request-response)。
- 手順 3: [3 番目の要求のサンプル](#third-request)と[最後の応答](#third-request-response)。

簡潔にするため、サンプルの応答にはイベントのプロパティのサブセットのみを表示します。実際の呼び出しでは、ほとんどのイベント プロパティが返されます。

[次のラウンド](#example-2-retrieving-additional-changes)で行う操作も参照してください。

#### <a name="initial-request"></a>最初の要求

この例では、チャネルのメッセージは初めて同期されるため、最初の同期要求には状態トークンは含まれません。 このラウンドは、そのカレンダー ビュー内のすべてのイベントを返します。

要求では、オプションの要求ヘッダー (odata) が指定され、一度に 2 つのイベントが返されます。

<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$top=2
```

#### <a name="initial-request-response"></a>最初の要求の応答

応答には、2 つのメッセージと `skipToken` が含まれた `@odata.nextLink` 応答ヘッダーが含まれています。 `nextLink` URL は、取得するべきメッセージが他にもチャネルにあることを示します。

>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.nextLink": "/teams('id')/channels('id')/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from" : {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T07:40:20.152Z",
            "lastModifiedDateTime": "2019-03-06T07:40:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        },
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from" : {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T08:40:20.152Z",
            "lastModifiedDateTime": "2019-03-06T08:40:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        }
    ]
}
```

#### <a name="second-request"></a>2 番目の要求

2 番目の要求では、前の応答で返された `nextLink` URL が指定されます。 最初の要求でのものと同じ top パラメーターを指定する必要はない点に注意してください。これは、`skipToken` URL の `nextLink` によってこれらのパラメーターがエンコードされて含まれるためです。

<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d
```

#### <a name="second-request-response"></a>2 番目の要求の応答

2 番目の応答には、次の 2 つのメッセージと `@odata.nextLink` を含む `skipToken` 応答ヘッダーが返されます。これは、取得するべきメッセージが他にもチャネルにあることを示します。

>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.nextLink": "/teams('id')/channels('id')/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from" : {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T09:40:20.152Z",
            "lastModifiedDateTime": "2019-03-06T09:40:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        },
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from" : {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T09:50:20.152Z",
            "lastModifiedDateTime": "2019-03-06T09:50:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        }
    ]
}
```

#### <a name="third-request"></a>3 番目の要求

3 番目の要求は、最後の同期要求から返された最新の `nextLink` を引き続き使用します。

<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d
```

#### <a name="third-request-response"></a>3 番目の要求の応答

3 番目の応答には、チャネルの残りのメッセージと `deltaToken` を含む `@odata.deltaLink` 応答ヘッダーが返されます。これは、チャネルのすべてのメッセージが読まれたことを示します。 この`deltaLink` URL を保存し、次のラウンドでこの時点以降のすべての新しいメッセージのクエリを行うために使用します。

>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.deltaLink": "/teams('id')/channels('id')/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from" : {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T10:40:20.152Z",
            "lastModifiedDateTime": "2019-03-06T10:40:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        }
    ]
}
```

### <a name="example-2-retrieving-additional-changes"></a>例 2: 追加の変更を取得する

前回のラウンドの最後の応答からの `deltaLink` を使用すると、それ以降にそのチャネルで (追加または更新によって) 変更されたこれらのメッセージのみを取得できます。 応答で同じ最大ページ サイズを維持することを前提とすると、要求は次のようになります。

#### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d
```

#### <a name="response"></a>応答

>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.deltaLink": "/teams('id')/channels('id')/messages/delta?$deltatoken=c3RhcnRUaW1l5Ti1NTEyODc1ODB0OTAyXGFdZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from" : {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T10:40:20.152Z",
            "lastModifiedDateTime": "2019-03-06T10:40:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Channel messages: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    ]
}
-->
