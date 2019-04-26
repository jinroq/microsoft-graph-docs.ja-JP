---
title: 'group: delta'
description: グループメンバーシップの変更を含む、新しく作成、更新、または削除されたグループを取得します。グループコレクション全体の完全な読み取りを実行する必要はありません。 詳細については、「デルタクエリの使用」を参照してください。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: ff525bf807cf7f4d2932aad30f61dab157dc6619
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329717"
---
# <a name="group-delta"></a>group: delta

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

グループメンバーシップの変更を含む、新しく作成、更新、または削除されたグループを取得します。グループコレクション全体の完全な読み取りを実行する必要はありません。 詳細については、「[デルタクエリの使用](/graph/delta-query-overview)」を参照してください。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Group.Read.All、Group.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Group.Read.All、Group.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

変更の追跡を開始するには、グループ リソースにデルタ関数を含む要求を実行します。

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a>クエリ パラメーター

グループで変更の追跡を実行するときには、1 つまたは複数の **delta** 関数の呼び出しが必要になります。クエリ パラメーター (`$deltatoken` および `$skiptoken` 以外) を使用する場合は、そのパラメーターを最初の **delta** 要求に指定する必要があります。指定されたパラメーターは、Microsoft Graph を使って自動的にエンコードされ、応答の `nextLink` または `deltaLink` URL のトークン部分として指定されます。

必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。

その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。

| クエリ パラメーター | 種類  |説明|
|:---------------|:--------|:----------|
| $deltatoken | string | 同じグループ コレクションの前の**デルタ**関数呼び出しの `deltaLink` URL で[状態トークン](/graph/delta-query-overview)が返され、その変更追跡のラウンドが完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。|
| $skiptoken | string | 前の**デルタ**関数呼び出しの `nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じグループ コレクションに追跡すべき変更が他にもあることを示します。 |

### <a name="odata-query-parameters"></a>OData クエリ パラメーター

このメソッドは、応答をカスタマイズするためのオプションの OData クエリパラメーターをサポートします。

- 任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。*Id* プロパティは常に返されます。
- を使用`$expand=members`して、メンバーシップの変更を取得することができます。
- 次のサポートに`$filter`制限があります。
  - サポートされている唯一の `$filter` 式は、特定のオブジェクトでの変更を追跡する `$filter=id+eq+{value}` です。 複数のオブジェクトをフィルター処理することができます。 たとえば、`https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'` などです。 フィルター処理されるオブジェクトには 50 の数量制限があります。

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 説明|
|:---------------|:----------|
| Authorization  | Bearer &lt;token&gt;|
| Content-Type  | application/json |
| Prefer | 戻り値 = 最小 <br><br>を`deltaLink`使用する要求でこのヘッダーを指定すると、最後のラウンド以降に変更されたオブジェクトプロパティのみが返されます。 省略可能。 |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

### <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) コレクション オブジェクトを返します。 応答には、 `nextLink` url または`deltaLink` url のいずれかの状態トークンも含まれます。

- URL が`nextLink`返される場合は、次のようになります。
  - これは、セッションで取得するデータのページが他にもあることを示しています。 アプリケーションは、応答に`nextLink` `deltaLink` url が含まれるまで、url を使用して要求を引き続き行います。
  - 応答には、初期デルタクエリ要求と同じプロパティセットが含まれています。 これにより、デルタサイクルを開始するときに、オブジェクトの現在の完全な状態を取得できます。

- URL が`deltaLink`返される場合は、次のようになります。
  - これは、返されるリソースの既存の状態に関するデータがないことを示します。 `deltaLink` URL を保存して使用し、次のラウンドでのリソースの変更について学習します。
  - `Prefer:return=minimal`ヘッダーを指定することもできます。これは、が発行`deltaLink`されてから変更されたプロパティのみを応答値に含めることを選択することです。

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a>Default: 初期デルタ要求と同じプロパティを返す

既定では、次の`deltaLink`方法`nextLink`で、を使用して、または初期デルタクエリで選択されたものと同じプロパティを返すことができます。

- プロパティが変更されている場合、新しい値は応答に含まれます。 これには、null 値に設定されているプロパティが含まれます。
- プロパティが変更されていない場合は、古い値が応答に含まれます。
- プロパティが設定されていない場合は、応答には含まれません。


> **注:** この動作では、応答を見ることで、プロパティが変更されているかどうかを判断することはできません。 また、次の[2 番目の例](#request-2)に示すように、デルタ応答は、すべてのプロパティ値を含むため、サイズが大きくなる傾向があります。

#### <a name="alternative-return-only-the-changed-properties"></a>代替方法: 変更されたプロパティのみを返す

オプションの要求ヘッダーを追加`prefer:return=minimal`する--次のような動作になります。

- プロパティが変更されている場合、新しい値は応答に含まれます。 これには、null 値に設定されているプロパティが含まれます。
- プロパティが変更されていない場合、プロパティは応答には含まれません。 (既定の動作とは異なります)。

> **注:** このヘッダーは、デルタサイクルの`deltaLink`任意の時点で要求に追加できます。 ヘッダーは、応答に含まれているプロパティのセットにのみ影響し、デルタクエリの実行方法には影響しません。 次の[3 つ目の例](#request-3)を参照してください。

### <a name="example"></a>例

#### <a name="request-1"></a>要求 1

要求の例を次に示します。 パラメーターがない`$select`ので、プロパティの既定のセットが追跡されて返されます。
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta
```

#### <a name="response-1"></a>応答 1

次に、クエリの初期化で`deltaLink`取得した場合の応答の例を示します。

>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 実際の呼び出しではすべてのプロパティが返されます。
>
> グループ内の member オブジェクトの id を含む*メンバー @ delta*プロパティが存在することに注意してください。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups","@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvY1FSSc_",
  "value":[
    {
      "classification": "classification-value",
      "createdDateTime":"datetime-value",
      "description":"Test group 1",
      "displayName":"TestGroup1",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "693acd06-2877-4339-8ade-b704261fe7a0"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    }
  ]
}
```

#### <a name="request-2"></a>要求 2

次の例は、既定の応答動作を使用して、変更追跡の3つのプロパティを選択する最初の要求を示しています。
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description,mailNickname
```

#### <a name="response-2"></a>応答 2

次に、クエリの初期化で`deltaLink`取得した場合の応答の例を示します。 3つすべてのプロパティは応答に含まれていますが、 `deltaLink`取得した後に変更されたプロパティが不明であることに注意してください。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null,
      "mailNickname": "mailNickname-value"
    }
  ]
}
```

#### <a name="request-3"></a>要求 3

次の例は、変更追跡の3つのプロパティを選択する最初の要求を示しています。これには、次のような最低限の応答動作があります。
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```

#### <a name="response-3"></a>応答 3

次に、クエリの初期化で`deltaLink`取得した場合の応答の例を示します。 プロパティは含ま`mailNickname`れていません。つまり、最後のデルタクエリ以降変更されていないことに注意してください。`displayName`と`description`は、その値が変更されたことを意味します。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null
    }
  ]
}
```

## <a name="see-also"></a>関連項目

- [デルタクエリを使用して、Microsoft Graph データの変更を追跡](/graph/delta-query-overview)します。
- [グループに対する増分の変更を取得](/graph/delta-query-groups)します。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
