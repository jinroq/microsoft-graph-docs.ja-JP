---
title: 'group: delta'
description: Get を新しく作成するには、更新、またはグループ メンバーシップの変更を含むグループ全体のコレクションのすべての読み取りを実行しなくても、グループを削除します。 詳細については、デルタのクエリを使用するを参照してください。
localization_priority: Normal
ms.openlocfilehash: d9032b6066184ddf993f7fa4645cae00ed1d48b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815142"
---
# <a name="group-delta"></a>group: delta
Get を新しく作成するには、更新、またはグループ メンバーシップの変更を含むグループ全体のコレクションのすべての読み取りを実行しなくても、グループを削除します。 詳細については、[デルタのクエリを使用する](/graph/delta-query-overview)を参照してください。

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
| $deltatoken | 文字列 | 同じグループ コレクションの前の**デルタ**関数呼び出しの `deltaLink` URL で[状態トークン](/graph/delta-query-overview)が返され、その変更追跡のラウンドが完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。|
| $skiptoken | 文字列 | 前の**デルタ**関数呼び出しの `nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じグループ コレクションに追跡すべき変更が他にもあることを示します。 |

### <a name="odata-query-parameters"></a>OData クエリ パラメーター

このメソッドは、応答をカスタマイズするためのオプションの OData クエリ パラメーターをサポートします。

- 任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。*Id* プロパティは常に返されます。
- 使用することができます`$expand=members`のメンバーシップの変更を取得します。
- サポートが制限されて`$filter`。
  - サポートされている唯一の `$filter` 式は、特定のオブジェクトでの変更を追跡する `$filter=id+eq+{value}` です。 複数のオブジェクトをフィルター処理することができます。 たとえば、`https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'` などです。 フィルター処理されるオブジェクトには 50 の数量制限があります。

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 説明|
|:---------------|:----------|
| Authorization  | Bearer &lt;token&gt;|
| Content-Type  | application/json |
| Prefer | 返す最小 = <br><br>このヘッダーを指定する要求を使用すると、`deltaLink`最後のラウンド以降に変更されたオブジェクトのプロパティのみを返します。 省略可能。 |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

### <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) コレクション オブジェクトを返します。 応答には、次のいずれかの状態のトークンも含まれています、`nextLink`の URL、または`deltaLink`URL です。

- 場合、`nextLink`の URL が返されます。
  - これは、他のページのセッションで取得するデータがあることを示します。 アプリケーションの継続を使用して要求を作成する、`nextLink`までの URL を`deltaLink`URL が応答に含まれています。
  - 応答には、同じ一連最初のデルタ ・ クエリ要求のようにプロパティにはが含まれています。 これにより、デルタ ・ サイクルを開始するときに、オブジェクトのすべての現在の状態をキャプチャすることができます。

- 場合、`deltaLink`の URL が返されます。
  - これは、返されるリソースの既存の状態に関するデータがあることを示します。 保存し、使用して、`deltaLink`について学習するための URL は次のラウンドでリソースを変更します。
  - 指定の選択肢がある場合、`Prefer:return=minimal`時間以降に変更されたプロパティのみの応答の値に追加する、ヘッダー、`deltaLink`が発行されました。

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a>既定値: は、最初のデルタ ・ リクエストと同じプロパティを返す

既定では、要求を使用して、`deltaLink`または`nextLink`次のように最初のデルタ ・ クエリで選択したのと同じプロパティを返します。

- プロパティが変更された場合は、応答に新しい値が含まれます。 これには、null 値に設定されているプロパティが含まれます。
- プロパティが変更されていない場合は、応答に古い値が含まれます。
- プロパティの場合は、含まれませんの応答ですべての前に設定されています。


> **注:** この現象に関して、応答を見ることはできませんプロパティを変更するかどうかどうかを確認します。 また、デルタの反応をする大規模なすべてのプロパティ値が含まれているため、次の[2 番目の例](#request-2)に示すように傾向があります。

#### <a name="alternative-return-only-the-changed-properties"></a>: 別の方法が変更されたプロパティのみを返す

オプションの要求ヘッダーでは - を追加する`prefer:return=minimal`の次の動作の結果します。

- プロパティが変更された場合は、応答に新しい値が含まれます。 これには、null 値に設定されているプロパティが含まれます。
- プロパティが変更されていない場合は、プロパティが含まれていない応答ですべての。 (既定の動作と異なります)

> **注:** ヘッダーを追加することができます、`deltaLink`デルタ ・ サイクルの時間内の任意の時点で要求します。 ヘッダーの応答に含まれるプロパティのセットにのみ影響し、デルタ ・ クエリを実行する方法には影響しません。 次の[3 番目の例](#request-3)を参照してください。

### <a name="example"></a>例

#### <a name="request-1"></a>要求 1

要求の例を次に示します。 ありません`$select`パラメーター、プロパティの既定のセットが追跡され、返されるようにします。
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

#### <a name="response-1"></a>応答 1

使用すると、次の応答の例では`deltaLink`クエリの初期化から取得します。

>**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。 実際の呼び出しではすべてのプロパティが返されます。
>
> グループ内のメンバー オブジェクトの id が含まれている*members@delta*プロパティが存在することに注意してください。

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

次の使用例は、変更の追跡、応答の既定の動作で 3 つのプロパティを選択する最初の要求を示しています。
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
```

#### <a name="response-2"></a>応答 2

使用すると、次の応答の例では`deltaLink`クエリの初期化から取得します。 応答ですべての 3 つのプロパティが含まれますし、以降に変更されているどれが不明、`deltaLink`を取得しました。

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

次の使用例は、3 つのプロパティの変更履歴の記録を最小限に抑える別の応答の動作を選択する最初の要求を示しています。
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```

#### <a name="response-3"></a>応答 3

使用すると、次の応答の例では`deltaLink`クエリの初期化から取得します。 なお、`mailNickname`プロパティが含まれていないことを意味するは、前回のデルタ ・ クエリは変更されていません。`displayName`と`description`は、値が変更されたことを意味します。

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

- [グラフ データの変更を追跡するためにデルタのクエリを使用します](/graph/delta-query-overview)。
- [グループの増分の変更を取得](/graph/delta-query-groups)します。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
