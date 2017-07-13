# クエリ パラメーターを使用して応答をカスタマイズする
<a id="use-query-parameters-to-customize-responses" class="xliff"></a>

Microsoft Graph にはオプションのクエリ パラメーターがあり、応答で返されるデータの量を指定したり制御するために使用できます。次のクエリ パラメーターがサポートされています。

|名前|説明|例 (例をクリックして [Graph エクスプローラー][graph-explorer]で試行します)
|:---------------|:--------|:-------|
|[$filter](#filter)|結果 (行) をフィルターします。|[`/users?$filter=startswith(givenName,'J')`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)
|[$select](#select)|プロパティ (列) をフィルターします。|[`/users?$select=givenName,surname`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0)
|[$expand](#expand)|関連リソースを取得します。|[`/groups/{id}?$expand=members`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups/22be6ccb-15a5-459f-94ac-d1393bdd9e66?$expand=members&method=GET&version=v1.0)
|[$orderby](#orderby)|結果を並べます。|[`/users?$orderby=displayName,userPrincipalName desc`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$orderby=displayName,userPrincipalName%20DESC&method=GET&version=v1.0)
|[$top](#top)|結果を制限します。通常、`$skipToken` と一緒に使用されます。|[`/users?$top=2`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0)
|[$skipToken](#skiptoken)|結果のページを取得するために `$top` と一緒に使用されます。|例については、$top クエリの `nextLink` を参照してください。
|[$count](#count)|一致するリソースの総数を取得します。|[`/me/messages?$top=2&$count=true`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0)
<!-- TODO: figure out whether $search is actually used
|[`$search`](#search)|A property and value pair separated by a colon.|
-->

これらのパラメーターは、[OData V4 クエリ言語][odata-query]と互換性があります。

> **注:**`beta` エンドポイントでは、`$` プレフィックスはオプションです。たとえば、`$filter` の代わりに、`filter` を使用しても同じです。詳細および例については、「[Microsoft Graph における $ プレフィックスのないクエリ パラメーターのサポート](http://dev.office.com/queryparametersinMicrosoftGraph)」を参照してください。

**クエリ パラメーターのエンコード:**

クエリ パラメーターの値はパーセント エンコードされる必要があります。これを行ううえで役立つ HTTP クライアント、ブラウザー、およびツールが多くあります (たとえば [Graph エクスプローラー][graph-explorer])。クエリが失敗する場合、クエリ パラメーターの値が適切にエンコードされていないことがその理由の 1 つとして考えられます。

エンコードされていない URL は、次のようになります。

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

正しくエンコードされている URL は、次のようになります。

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## filter
<a id="filter" class="xliff"></a>

`$filter` は、コレクションのサブセットのみを取得するために使用できます。たとえば、表示名が `J` で始まるユーザーを検索するには、`startswith` を使用します。

[Graph エクスプローラーで試す](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)

**要求:**

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

**応答:**

```json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users",
    "value": [
        {
            "id": "e013b9f3-a1ab-48d1-907b-e716c39d6363",
            "businessPhones": [
                "4255550100"
            ],
            "displayName": "Jan Madden",
            "givenName": "Jan",
            "jobTitle": null,
            "mail": "demo32@a830edad9050849NDA1.onmicrosoft.com",
            "mobilePhone": null,
            "officeLocation": null,
            "preferredLanguage": null,
            "surname": "Madden",
            "userPrincipalName": "demo32@a830edad9050849NDA1.onmicrosoft.com"
        },
        {
            "id": "89efe8ed-d141-4151-a3e4-570a70022dff",
            "businessPhones": [
                "+1 425 555 0109"
            ],
            "displayName": "Janet Schorr",
            "givenName": "Janet",
            "jobTitle": "Product Marketing Manager",
            "mail": "janets@a830edad9050849NDA1.onmicrosoft.com",
            "mobilePhone": null,
            "officeLocation": "18/2111",
            "preferredLanguage": null,
            "surname": "Schorr",
            "userPrincipalName": "janets@a830edad9050849NDA1.onmicrosoft.com"
        },
        ...
    ]
}
```

`$filter` の構文は非常に豊富かつ多彩であり、多くの演算子が組み込まれています。論理演算子には、等号 (`eq`)、不等号 (`ne`)、より大 (`gt`)、以上 (`gte`)、AND (`and`)、OR (`or`)、NOT (`not`) などが含まれます。算術演算子には、加算 (`add`)、減算 (`sub`) などが含まれます。文字列演算子には、次の値を含む (`contains`)、次の文字列で始まる (`startswith`) などが含まれます。ラムダ演算子には、一部 (`any`)、すべて (`all`).が含まれます。`$filter` 構文の詳細については、「[OData プロトコル][odata-filter]」を参照してください。


## select
<a id="select" class="xliff"></a>

コレクションまたは個別のエンティティで既定のセットの代わりに返される別のプロパティのセットを指定するには、`$select` クエリ パラメーターを使用します。`$select` パラメーターにより、返される既定のセットのサブセットまたはスーパーセットを選択できます。たとえば、メッセージを取得する場合、メッセージの `from` と `subject` プロパティだけが返されるように選択することができます。

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<!--For example, when retrieving the children of an item on a drive, you want to select that only the `name` and `size` properties of items are returned.

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name,size
```

By submitting the request with the `$select=name,size` query string, the objects
in the response will only have those property values included.

```json
{
  "value": [
    {
      "id": "13140a9sd9aba",
      "name": "Documents",
      "size": 1024
    },
    {
      "id": "123901909124a",
      "name": "Pictures",
      "size": 1012010210
    }
  ]
}
```-->

## expand
<a id="expand" class="xliff"></a>

Microsoft Graph API 要求では、参照されている項目のオブジェクトまたはコレクションへのナビゲーションは自動的には展開されません。これは仕様です。サービスからの応答を生成するためのネットワーク トラフィックと時間を減らすためです。しかし、応答にそれらの結果を含めることが必要な場合があります。

`$expand` クエリ文字列パラメーターを使用して、子オブジェクトまたはコレクションを展開しそれらの結果を含めるよう API に指示できます。

たとえば、ルート ドライブ情報とドライブの最上位レベルの子項目を取得するには、`$expand` パラメーターを使用します。またこの例では、子項目の `id` および `name` プロパティだけを返すために、[`$select`](#select) ステートメントも使用しています。

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

> **注:**要求に対して拡張されるオブジェクトの最大数は 20 です。また、[`user`](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) のリソースにクエリを実行する場合、プロパティを取得するために `$expand` を使用すると子オブジェクトまたはコレクションを一度に 1 つずつしか取得できません。次の例では `user` オブジェクトを取得します。それぞれは展開された `directReports` コレクション内で最大 20 個の `directReport` オブジェクトを取得します。

```http
GET https://graph.microsoft.com/v1.0/users?$expand=directReports
```

他のいくつかのリソースにも制限がある場合があるため、潜在的なエラーを常にチェックします。

## orderby
<a id="orderby" class="xliff"></a>

Microsof Graph API から返される項目の並べ替え順序を指定するには、`$orderby` クエリ パラメーターを使用します。

たとえば、組織のユーザーを表示名順で戻す場合、構文は次のようになります。

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```

複合型のエンティティでも並べ替えが可能です。次の例では、メッセージを取得し、それらを `emailAddress` という複合型である `from` プロパティの `address` フィールドで並べ替えます。

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```

昇順または降順で結果を並べ替えるには、`asc` または `desc` のいずれかをスペースで区切ってフィールド名の後に追加します。たとえば `?$orderby=name%20desc` のようにします。

 > **注:**[`user`](../api-reference/v1.0/resources/user.md) リソースでクエリを実行する場合、`$orderby` は filter 式と組み合わせることはできません。

## top
<a id="top" class="xliff"></a>

結果セットに返す項目の最大数を指定するには、`$top` クエリ オプションを使用します。`$top` クエリ パラメーターは、コレクションのサブセットを指定します。このサブセットは、最初の N 項目のみが選択されて形成されます。ここで、N はこのクエリ パラメーターで指定される正の整数です。たとえば、ユーザーのメールボックスの最初の 5 つのメッセージを返す構文は、次のとおりです。

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

## skip
<a id="skip" class="xliff"></a>

コレクション内の項目を取得する前にスキップする項目数を設定するには、`$skip` クエリ パラメーターを使用します。たとえば、作成日付順に並べ替えたイベントを 21 番目から戻す構文は、次のとおりです。

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```

## skipToken
<a id="skiptoken" class="xliff"></a>

Graph データの 2 番目およびそれ以降のページを要求するには、`$skipToken` クエリ パラメーターを使用します。(通常はサーバー サイドのページングによって) Graph が結果の一部のサブセットを返したときに、`$skipToken` クエリ パラメーターは Graph から返される URL で提供されます。それはコレクション内の、サーバーが結果の送信を終了したポイントを指定し、それから Graph に返され、結果の送信をどこから再開する必要があるかを指定します。たとえば、`$skipToken` クエリ パラメーターの値によって、コレクションの 10 番目の項目を指定したり、50 個の項目を含むコレクション内の 20 番目の項目やコレクション内の他の任意の位置の項目を指定できます。

応答によっては、`@odata.nextLink` の値が表示される場合があります。それらには、`$skipToken` 値が含まれる場合があります。`$skipToken` 値は、次の結果セットを再開する位置をサービスに示すマーカーのようなものです。`displayName` 順の、ユーザーが要求された応答からの `@odata.nextLink` 値の例は次のとおりです。

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$orderby=displayName&$skiptoken=X%2783630372100000000000000000000%27"
```

組織のユーザーの次のページを返すには、次の構文を使用します。

```http
GET  https://graph.microsoft.com/v1.0/users?$orderby=displayName&$skiptoken=X%2783630372100000000000000000000%27
```

## count
<a id="count" class="xliff"></a>

クエリ パラメーターとして `$count` を使用し、次の例のように、Graph から返されるデータ値のページにコレクション内の項目数の合計を含めます。

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

これは `contacts` コレクションおよび `@odata.count` プロパティにある `contacts` コレクション内の項目数の両方を返します。

>**注:**これは、[`directoryObject`](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/directoryobject) コレクションではサポートされていません。

## search
<a id="search" class="xliff"></a>

要求の結果を検索条件と一致するものに制限するには、`$search` クエリ パラメーターを使用します。

> **注:**現在の検索対象は、[メッセージ](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/message) コレクションと[人物](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/person)コレクション**だけ**です。`$search` 要求は最大 250 まで結果を返します。検索要求では [`$filter`](#filter) も [`$orderby`](#orderby) も使用できません。

検索条件は、高度な検索テクニック (AQS) を使用して表現されます。結果は、メッセージが送信された日時で並べ替えられます。

`$search` で `message` に対する次のプロパティを指定できます: `attachments`、`bccRecipients`、`body`、`category`、`ccRecipients`、`content`、`from`、`hasAttachments`、`participants`、`receivedDateTime`、`sender`、`subject`、`toRecipients`

メッセージで検索を行うときに値のみ指定した場合、検索は既定の検索プロパティである `from`、`subject` および `body` に基づいて行われます。

次の例は、サインイン中のユーザーの受信トレイにあるメッセージのうち、既定の 3 つの検索プロパティのいずれかに "pizza" が含まれるメッセージをすべて返します。

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

次の例は、ユーザーの受信トレイにあるメッセージのうち、特定のメール アドレスから送信されたメッセージをすべて検索します。

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```

[graph-explorer]: https://graph.microsoft.io/en-us/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
