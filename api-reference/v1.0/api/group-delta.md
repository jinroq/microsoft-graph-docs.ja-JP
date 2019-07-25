---
title: 'group: delta'
description: グループメンバーシップの変更を含む、新しく作成、更新、または削除されたグループを取得します。グループコレクション全体の完全な読み取りを実行する必要はありません。 詳細については、「デルタクエリの使用」を参照してください。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 2e2ab2c2842b6bd2423a57c54eebde03664f8a7c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890864"
---
# <a name="group-delta"></a>group: delta
グループメンバーシップの変更を含む、新しく作成、更新、または削除されたグループを取得します。グループコレクション全体の完全な読み取りを実行する必要はありません。 詳細については、「[デルタクエリの使用](/graph/delta-query-overview)」を参照してください。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.accessasuser.all。すべて、ディレクトリの読み取り、すべてのディレクトリを読み取ることができます。すべてを示します。.  |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | 。すべて、ディレクトリの読み取り、すべてのディレクトリの読み取り、すべてのディレクトリを取得します。 |

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
- `$filter` に対するサポートには制限があります。
  - サポートされている唯一の `$filter` 式は、特定のオブジェクトでの変更を追跡する `$filter=id+eq+{value}` です。 複数のオブジェクトをフィルター処理することができます。 たとえば、`https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'` などです。 フィルター処理されるオブジェクトには 50 の数量制限があります。

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 説明|
|:---------------|:----------|
| Authorization  | Bearer &lt;token&gt;|
| Content-Type  | application/json |
| Prefer | return=minimal. <br><br>このヘッダーを指定する要求を使用すると、`deltaLink` は、最後のラウンド以降に変更されたオブジェクトのプロパティのみを返します。 省略可能です。 |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

### <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) コレクション オブジェクトを返します。 応答には、 `nextLink` url または`deltaLink` url のいずれかの状態トークンも含まれます。

- もし`nextLink` URL が返された場合:
  - セッションで取得するデータに追加ページがあることを示しています。 アプリケーションは`deltaLink` URL が応答に含まれるまで`nextLink` URLを使用して要求を続けます。
  - 応答には、最初のデルタクエリ要求と同じ一連のプロパティが含まれています。 これにより、デルタサイクルを開始するときに、オブジェクトの現在の完全な状態をキャプチャできます。

- もし`deltaLink` URL が返された場合:
  - これは、返されるリソースの既存の状態に関するデータがこれ以上ないことを示します。 `deltaLink` URL を、次回のラウンドでリソースへの変更について学ぶために保存して使ってください。
  - `Prefer:return=minimal` ヘッダーを指定して、`deltaLink`発行後に変更されたプロパティのみをレスポンス値に含めるように選択することもできます。

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a>デフォルト：初期デルタリクエストと同じプロパティを返します

デフォルトでは、`deltaLink`または`nextLink`を使用したリクエストは、最初のデルタクエリで選択されたものと同じプロパティを次のように返します:

- プロパティを変更した場合は、応答には新しい値が含まれます。 これには、null 値に設定されているプロパティが含まれます。
- プロパティが変更されていない場合は、古い値が応答に含まれています。
- プロパティが設定されたことがない場合は、応答にまったく含まれません。


> **注意:** この動作では、応答を見ても、プロパティが変化しているかどうかを判断することはできません。 また、デルタ応答は-以下の[2番目の例](#request-2)に示されるようにすべてのプロパティ値を含むため、大きくなる傾向があります 。

#### <a name="alternative-return-only-the-changed-properties"></a>代替案：変更されたプロパティのみを返す

オプションのリクエストヘッダを追加すると、- `prefer:return=minimal` - 次のようになります:

- プロパティを変更した場合は、応答には新しい値が含まれます。 これには、null 値に設定されているプロパティが含まれます。
- プロパティが変更されていない場合、そのプロパティは応答にまったく含まれません。 (既定の動作と異なる)

> **注意:** ヘッダーは、デルタサイクルのどの時点でも `deltaLink`要求に追加できます。 ヘッダーは応答に含まれる一連のプロパティにのみ影響し、デルタクエリの実行方法には影響しません。 以下の[三番目の例](#request-3)を参照してください。

### <a name="example"></a>例

#### <a name="request-1"></a>要求 1

要求の例を次に示します。 `$select`パラメータがないため、デフォルトのプロパティセットが追跡されて返されます。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-1"></a>応答 1

以下は、クエリ初期化から取得した`deltaLink` を使用した場合の応答の例です。

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups","@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvY1FSSc_",
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

次の例は、デフォルトの応答動作で、変更追跡のために3つのプロパティを選択する最初の要求を示しています。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delta_with_select"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-with-select-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-with-select-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-with-select-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-with-select-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-2"></a>応答 2

以下は、クエリ初期化から取得した`deltaLink` を使用した場合の応答の例です。 3つのプロパティすべてがレスポンスに含まれており、`deltaLink`が取得されてからどのプロパティが変更されたのかはわかりません。

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
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

次の例は、最初のリクエストが代替の最小限の応答の変更追跡のために3つのプロパティを選択していることを示しています。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delta_minimal"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-minimal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-3"></a>応答 3

以下は、クエリ初期化から取得した`deltaLink` を使用した場合の応答の例です。 この`mailNickname`プロパティは含まれていないことに注意してください 。つまり、最後のデルタクエリ以降変更されていません;`displayName`と`description` が含まれており、それらの値は変更されていることを意味します。

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null
    }
  ]
}
```

## <a name="see-also"></a>関連項目

- [デルタクエリを使用してMicrosoft Graphデータの変更を追跡します](/graph/delta-query-overview)。
- [グループに対する増分の変更を取得](/graph/delta-query-groups)します。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
