# <a name="use-query-parameters-to-customize-responses"></a>クエリ パラメーターを使用して応答をカスタマイズする

Microsoft Graph にはオプションのクエリ パラメーターがあり、応答で返されるデータの量を指定したり制御したりするために使用できます。次のクエリ パラメーターがサポートされています。

|名前|説明|例 (例をクリックして [Graph エクスプローラー][graph-explorer]で試行します)
|:---------------|:--------|:-------|
|[$count](#count)|一致するリソースの総数を取得します。|[`/me/messages?$top=2&$count=true`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0)
|[$expand](#expand)|関連リソースを取得します。|[`/groups?$expand=members`](https://developer.microsoft.com/graph/graph-explorer?request=groups$expand=members&method=GET&version=v1.0)
|[$filter](#filter)|結果 (行) をフィルターします。|[`/users?$filter=startswith(givenName,'J')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)
|[$orderby](#orderby)|結果を並べます。|[`/users?$orderby=displayName desc`](https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0)
|[$search](#search)| 検索条件に基づいて結果を返します。現在、`messages` と `person` のコレクションでサポートされています。|[`/me/messages?$search=pizza`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0)
|[$select](#select)|プロパティ (列) をフィルターします。|[`/users?$select=givenName,surname`](https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0)
|[$skip](#skip)|結果セットにインデックスを作成します。また一部の API でページングを実装するために使用されており、`$top` と組み合わせて結果を手動でページングすることもできます。  | [`/me/messages?$skip=11`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0)
|[$skipToken](#skiptoken)|複数ページにわたる結果セットから、結果の次のページを取得します。(一部の API では代わりに `$skip` を使用します。) | `https://graph.microsoft.com/v1.0/users?$skiptoken=X%274453707402000100000017 ... 65612D643839392D343230372D613033662D306332623836633432363932B900000000000000000000%27`
|[$top](#top)|結果のページ サイズを設定します。 |[`/users?$top=2`](https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0)

これらのパラメーターは、[OData V4 クエリ言語][odata-query]と互換性があります。すべての Microsoft Graph API で全部のパラメーターがサポートされているわけではなく、`v1.0` エンドポイントと `beta` エンドポイントの間でサポートが大幅に異なる場合があります。 

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

## <a name="count"></a>count

`$count` クエリ パラメーターを使用し、Microsoft Graph から返されるデータ値のページにコレクション内の項目数の合計を含めます。 

たとえば、次のような要求によって、現在のユーザーの `contacts` コレクションと、`@odata.count` プロパティ内の `contacts` コレクションのアイテム数の両方が返されます。

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[Graph エクスプローラーで試す](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


>**注:** `$count` は、[ユーザー](../api-reference/v1.0/resources/user.md)や[グループ](../api-reference/v1.0/resources/group.md)のコレクションのような、[`directoryObject`](../api-reference/v1.0/resources/directoryobject.md) から派生したリソースのコレクションに対してはサポートされていません。

## <a name="expand"></a>expand

Microsoft Graph リソースの多くは、宣言されているリソースのプロパティと、他のリソースとのリレーションシップの両方を公開します。これらのリレーションシップは、参照プロパティまたはナビゲーション プロパティとも呼ばれ、1 つのリソースまたはリソースのコレクションのいずれかを参照することができます。たとえば、ユーザーのメール フォルダー、マネージャー、直属の部下は、すべてリレーションシップとして公開されます。 

通常、単一の要求では、リソースの複数のプロパティ、またはリソースのリレーションシップの 1 つのいずれかに対してクエリを実行できますが、両方は行えません。`$expand` クエリ文字列パラメーターを使用して、展開されているリソース、または単一のリレーションシップ (ナビゲーション プロパティ) で参照されているコレクションを結果に含めることができます。

次の例では、ドライブ内のトップレベルの子項目と共に、ルート ドライブ情報を取得します。

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[Graph エクスプローラーで試す](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

いくつかのリソース コレクションで、`$select` パラメーターを追加すれば、展開されたリソースで返されるプロパティを指定することもできます。次の使用例は前の例と同じクエリを実行しますが、[`$select`](#select) ステートメントを使用して、展開されている子項目に返されるプロパティを `id` プロパティと `name` プロパティに限定します。

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

[Graph エクスプローラーで試す](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children($select=id,name)&method=GET&version=v1.0)

> **注:** すべてのリレーションシップとリソースで、`$expand` クエリ パラメーターがサポートされているわけではありません。たとえば、ユーザーの `directReports`、`manager`、`memberOf` の各リレーションシップを展開できますが、その `events`、`messages`、`photo` のリレーションシップは展開できません。すべてのリソースまたはリレーションシップで、`$select` を使用して展開されたアイテムがサポートされているわけではありません。 
> 
> [ユーザー](../api-reference/v1.0/resources/user.md)や[グループ](../api-reference/v1.0/resources/group.md)のような、[directoryObject](../api-reference/v1.0/resources/directoryobject.md) から派生した Azure AD リソースの場合、`$expand` は `beta` でのみサポートされており、通常は展開されているリレーションシップに対し最大 20 個のアイテムを返すことができます。

## <a name="filter"></a>filter

`$filter` クエリ パラメーターを使用して、コレクションのサブセットのみを取得します。 

たとえば、表示名が「J」という文字で始まるユーザーを検索するには、`startswith` を使用します。

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

[Graph エクスプローラーで試す](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)

`$filter` 演算子へのサポートは、お使いの Microsoft Graph API によって異なります。通常、次の論理演算子はサポートされています。等しい (`eq`)、等しくない (`ne`)、より大きい (`gt`)、以上 (`ge`)、より小さい (`lt`)、以下 (`le`)、かつ (`and`)、または (`or`)、否定 (`not`)。`startswith` 文字列の演算子はたいていサポートされています。`any` ラムダ演算子は、一部の API でサポートされています。いくつかの使用例について、下の表を参照してください。`$filter` 構文の詳細については、「[OData プロトコル][odata-filter]」を参照してください。  

次の表では、`$filter` クエリ パラメーター使用例を示します。

|説明|例 (例をクリックして [Graph エクスプローラー][graph-explorer]で試行します)|
|:--------|:-------|
|  複数のプロパティ間で Mary という名前を持つユーザーを検索します。 | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) |
| 2017 年 7 月 1 日以降に開始する、サインイン ユーザーのイベントすべてを取得します。 | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) |
| サインイン ユーザーが受信した特定のアドレスからの電子メールすべてを取得します。 | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) |
| 2017 年 4 月にサインイン ユーザーが受信した電子メールすべてを取得します。 | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) |
| サインイン ユーザーの受信トレイから未読メールをすべて取得します。 | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) |
| 組織内のすべての Office 365 グループの一覧 | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) |

> **注:** Azure AD リソースでは、次の `$filter` 演算子はサポートされていません: `ne`、`gt`、`ge`、`lt`、`le`、`not`。Microsoft Graph リソースでは現在、`contains` 文字列の演算子はサポートされていません。

## <a name="orderby"></a>orderby

`$orderby` クエリ パラメーターを使用して、Microsof Graph から返される項目の並べ替え順序を指定します。

たとえば、次の要求では組織のユーザーが表示名順で返されます。

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
[Graph エクスプローラーで試す](https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName&method=GET&version=v1.0)

複合型のエンティティでも並べ替えが可能です。次の要求では、メッセージを取得し、それらを `emailAddress` という複合型である `from` プロパティの `address` フィールドで並べ替えます。

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[Graph エクスプローラーで試す](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

昇順または降順で結果を並べ替えるには、`asc` または `desc` のいずれかをスペースで区切ってフィールド名の後に追加します。たとえば `?$orderby=name%20desc` のようにします。

一部の API では、複数のプロパティの結果を並べ替えることができます。たとえば、次のような要求ではユーザーの受信トレイ内のメッセージを、最初は送信者の名前で降順に並べ替え (Z から A)、次に件名で昇順 (既定) に並べ替えます。

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```
[Graph エクスプローラーで試す](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)


 > **注:** [ユーザー](../api-reference/v1.0/resources/user.md)や[グループ](../api-reference/v1.0/resources/group.md)のような、[directoryObject](../api-reference/v1.0/resources/directoryobject.md) から派生した Azure AD リソースの場合、`$orderby` 式と `$filter` 式を結合することはできません。 

## <a name="search"></a>search

`$search` クエリ パラメーターを使用して、要求の結果を検索条件と一致するものに制限します。

> **注:** 現在の検索対象は、[メッセージ](../api-reference/v1.0/resources/message.md) コレクションと[人物](../api-reference/v1.0/resources/person.md)コレクション**だけ**です。`$search` 要求は最大 250 まで結果を返します。検索要求では [`$filter`](#filter) も [`$orderby`](#orderby) も使用できません。

### <a name="using-search-on-message-collections"></a>`message` コレクションで $Search を使用する

メッセージの検索条件は、[高度な検索テクニック (AQS)](https://support.office.com/article/Search-Mail-and-People-in-Outlook-com-and-Outlook-on-the-web-for-business-88108edf-028e-4306-b87e-7400bbb40aa7) を使用して表現されます。結果は、メッセージが送信された日時で並べ替えられます。

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

### <a name="using-search-on-person-collections"></a>`person` コレクションで $Search を使用する

Microsoft Graph People API を使用してユーザーに最も関連のある人物を取得できます。関連性は、ユーザーのコミュニケーションとコラボレーション パターン、およびビジネスのリレーションシップによって決定されます。People API では、`$search` クエリ パラメーターがサポートされています。

[人物](../api-reference/v1.0/resources/person.md)リソースの `displayName` プロパティと `emailAddress` プロパティの両方で人物の検索を行います。検索は、あいまい一致のアルゴリズムを実装します。これにより、完全に一致する項目と、検索目的の推論に基づく結果が返されます。たとえば、サインイン ユーザーの `people` コレクション内で、"Tyler Lee" の表示名および tylerle@example.com というメール アドレスを持つユーザーを想定してください。次の検索はすべて、Tyler を含む検索結果を返します。

```http
GET https://graph.microsoft.com/v1.0/me/people?$search=tyler                //matches both Tyler's name and email
GET https://graph.microsoft.com/v1.0/me/people?$search=tylerle              //matches Tyler's email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle@example.com"  //matches Tyler's email. Note the quotes to enclose '@'.
GET https://graph.microsoft.com/v1.0/me/people?$search=tiler                //fuzzy match with Tyler's name 
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler lee"          //matches Tyler's name. Note the quotes to enclose the space.
```

特定のトピックに興味のある人物の検索を実行することもできます。ユーザーのメールのスレッドから引き出した推測に基づいて検索を実行します。たとえば、次の検索は、サインイン ユーザーに関連のある人物のうち、そのユーザーとの通信の中でピザに興味を示した人のコレクションを返します。検索語句を引用符で囲んでいることに注目してください。

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="topic:pizza"                
```

最後に、2 種類の検索式を組み合わせることによって、同じ要求内に人の検索とトピックの検索の両方をまとめることができます。

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="tyl topic:pizza"                
```
この要求は本質的には 2 つの検索を行います。サインイン ユーザーに関連する人物の `displayName` プロパティと `emailAddress` プロパティに対するあいまい検索、そしてユーザーに関連する人物に対する「ピザ」というトピックの検索です。次いで結果をランク付けし、並べ替え、返します。この検索は制限的ではありません。「tyl」とあいまい一致する人物、「ピザ」に関心を示す人物、または両方の結果を取得する可能性があります。

People API についてもっと知るには、「[関係する人の情報を取得する](./people_example.md)」を参照してください。  

## <a name="select"></a>select

`$select` クエリ パラメーターを使用して、個別リソースまたはリソースのコレクションの既定値とは異なるプロパティのセットを返します。$Select で、既定のプロパティのサブセットまたはスーパー セットを指定できます。

たとえば、サインイン ユーザーのメッセージを取得するとき、`from` プロパティと `subject` プロパティだけを返すよう指定できます。

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

[Graph エクスプローラーで試す](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$select=from,subject&method=GET&version=v1.0)

> **重要:**通常は、`$select` を使用して、クエリから返されるプロパティをお使いのアプリで必要なものだけに制限することをお勧めします。これは特に、クエリが大きな結果セットを返す可能性がある場合に該当します。行ごとに返されるプロパティを制限すれば、ネットワークの負荷を軽減し、アプリのパフォーマンスを向上させることができます。
>
> `v1.0`では、[ユーザー](../api-reference/v1.0/resources/user.md)と[グループ](../api-reference/v1.0/resources/group.md)のような、[directoryObject](../api-reference/v1.0/resources/directoryobject.md) から派生した一部の Azure AD リソースは、読み取り時に制限された既定値のプロパティ サブセットを返します。既定のセット以外のプロパティを返すには、これらのリソースに対して `$select` を使用する必要があります。  

## <a name="skip"></a>skip

コレクションを開始するときにスキップする項目数を設定するには、`$skip` クエリ パラメーターを使用します。たとえば、次の要求はユーザーのイベントを、コレクション内の 21 番目以降のイベントから作成日順で返します。

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
[Graph エクスプローラーで試す](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$orderby=createdDateTime&$skip=20&method=GET&version=v1.0)

> **注:** Outlook メール/カレンダーなどいくつかの Microsoft Graph API (`message`、`event`、`calendar`) は、`$skip` を使用してページングを実装します。クエリの結果が複数ページにまたがる場合、これらの API は`@odata:nextLink` プロパティと共に `$skip` パラメーターが含まれる URL を返します。この URL を使用して、結果の次のページに戻れます。詳細については、「[ページング](./paging.md)」を参照してください。

## <a name="skiptoken"></a>skipToken

要求の中には、サーバー側のページングを使用したり、応答におけるページ サイズを限定するために [`$top`](#top) パラメーターを使用したりすることによって、複数のデータ ページを返すものがあります。Microsoft Graph API の多くは、`skipToken` クエリ パラメーターを使用して、結果の後続のページを参照します。`$skiptoken` パラメーターは、結果の次のページを参照する不透明トークンを含んでおり、応答の `@odata.nextLink` プロパティで指定される URL で返されます。詳細については、「[ページング](./paging.md)」を参照してください。


## <a name="top"></a>top

`$top` クエリ パラメーターを使用して、結果セットのページ サイズを指定します。 

残りの結果セットにさらに項目がある場合、応答本文に `@odata.nextLink` パラメーターが含まれます。このパラメーターには、結果の次のページを取得するために使用できる URL が含まれています。詳細については、「[ページング](./paging.md)」を参照してください。 

たとえば、次の要求はユーザーのメールボックスの最初の 5 つのメッセージを返します。

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

[Graph エクスプローラーで試す](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=5&method=GET&version=v1.0)


## <a name="error-handling-for-query-parameters"></a>クエリ パラメーターのエラー処理

指定されたクエリ パラメーターがサポートされていない場合、一部の要求はエラー メッセージを返します。たとえば、`$expand` を `user/photo` のリレーションシップで使用することはできません。 

```http
https://graph.microsoft.com/beta/me?$expand=photo
```

```json
{
    "error":{
        "code":"ExpandNotSupported",
        "message":"Expand is not allowed for property 'Photo' according to the entity schema.",
        "innerError":{
            "request-id":"1653fefd-bc31-484b-bb10-8dc33cb853ec",
            "date":"2017-07-31T20:55:01"
        }
    }
}
```

ただし、要求で指定されたクエリ パラメーターが警告なしで失敗する可能性があるため、注意が必要です。これは、クエリ パラメーターがサポートされていない場合や、クエリ パラメーターの組み合わせがサポートされていない場合に起こり得ます。その場合、要求によって返されたデータを調べ、指定したクエリ パラメーターに期待どおりの効果があったかどうかを確認する必要があります。 

[graph-explorer]: https://developer.microsoft.com/graph/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356