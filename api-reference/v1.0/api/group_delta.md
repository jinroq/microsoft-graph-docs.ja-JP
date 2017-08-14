# <a name="group-delta"></a>group: delta

[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用すると、アプリケーションは、要求ごとにターゲット リソースをすべて読み取ることなく、新しく作成、更新、削除されたエンティティを検出できます。グループへの変更を検出するには、*デルタ*関数を使用して要求を実行します。詳細については、「[デルタ クエリの使用](../../../concepts/delta_query_overview.md)」をご覧ください。

## <a name="prerequisites"></a>前提条件

この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.Read.All* または *Group.ReadWrite.All*

## <a name="http-request"></a>HTTP 要求

変更の追跡を開始するには、グループ リソースにデルタ関数を含む要求を実行します。 

<!-- { "blockType": "ignored" } -->
```http
GET /groups/delta
```

### <a name="query-parameters"></a>クエリ パラメーター

グループの変更を追跡すると、1 つ以上の **デルタ**関数呼び出しのラウンドが発生します。任意のクエリ パラメーター (`$deltatoken` と `$skiptoken` 以外) を使用する場合は、最初の**デルタ**要求でこれを指定する必要があります。Microsoft Graph は、応答で提供される `nextLink` や `deltaLink` の URL のトークン部分に指定したパラメーターを自動的にエンコードします。必要なクエリ パラメーターを前もって指定しておくだけで済みます。それ以降の要求では、前の応答で `nextLink` や `deltaLink` の URL に必要なパラメーターが既にエンコードされ、含まれているため、この URL をコピーして適用します。

| クエリ パラメーター      | 種類   |説明|
|:---------------|:--------|:----------|
| $deltatoken | string | 同じグループ コレクションの前の**デルタ**関数呼び出しの `deltaLink` URL で[状態トークン](../../../concepts/delta_query_overview.md)が返され、その変更追跡のラウンドが完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。|
| $skiptoken | string | 前の**デルタ**関数呼び出しの `nextLink` URL で[状態トークン](../../../concepts/delta_query_overview.md)が返され、同じグループ コレクションに追跡すべき変更が他にもあることを示します。 |

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための OData クエリ パラメーターをサポートします。

- 任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。 
- デルタ クエリは、グループの `$select`、`$top`、`$expand` をサポートします。 
- `$orderby` に対するサポートには制限があります。サポートされている唯一の `$orderby` 式は、`$orderby=receivedDateTime+desc` です。`$orderby` 式を含めない場合、戻り値の順序は保証されません。 
- `$search` はサポートされていません。

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | Bearer &lt;token&gt;|
| Content-Type  | application/json |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

### <a name="response"></a>応答

成功した場合、このメソッドは `200, OK` 応答コードと、応答本文で [group](../resources/group.md) コレクション オブジェクトを返します。応答には、状態トークン (nextLink URL や deltaLink URL) も含まれます。

- nextLink URL が返される場合は、セッションに取得するデータの追加ページがあります。deltaLink URL が応答で返されるまで、アプリケーションは nextLink URL を使用して要求を実行し続けます。

- deltaLink URL が返される場合、返されるリソースの既存の状態に関するデータはありません。以降の要求では、アプリケーションは deltaLink URL を使用して、リソースへの変更点を確認します。

参照先:</br>
- 詳細については、「[デルタ クエリの使用](../../../concepts/delta_query_overview.md)」をご覧ください</br>
- 要求の例については、「[グループに対する増分の変更を取得する](../../../concepts/delta_query_groups.md)」をご覧ください。</br>
    
## <a name="example"></a>例
##### <a name="request"></a>要求
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

##### <a name="response"></a>応答
注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。

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
      "mail": "mail-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->