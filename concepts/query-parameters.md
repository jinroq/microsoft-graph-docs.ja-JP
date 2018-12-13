---
title: クエリ パラメーターを使用して応答をカスタマイズする
description: Microsoft Graph にはオプションのクエリ パラメーターがあり、応答で返されるデータの量を指定したり制御したりするために使用できます。次のクエリ パラメーターがサポートされています。
ms.openlocfilehash: e41a6e8d9cc42506985bd82f00bcdc4efaec8add
ms.sourcegitcommit: 2532b8dd7f2533d956e2600855b3daeabdd9b8ff
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/30/2018
ms.locfileid: "27092551"
---
# <a name="use-query-parameters-to-customize-responses"></a>クエリ パラメーターを使用して応答をカスタマイズする

Microsoft Graph にはオプションのクエリ パラメーターがあり、応答で返されるデータの量を指定したり制御したりするために使用できます。次のクエリ パラメーターがサポートされています。

>**注:** 例をクリックして [Graph エクスプローラー][graph-explorer]で試行します。

| 名前                     | 説明 | 例
|:-------------------------|:------------|:---------|
| [$count](#count-parameter)         | 一致するリソースの総数を取得します。 | [`/me/messages?$top=2&$count=true`][count-example]
| [$expand](#expand-parameter)       | 関連リソースを取得します。|[`/groups?$expand=members`][expand-example]
| [$filter](#filter-parameter)       | 結果 (行) をフィルターします。|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [$format](#format-parameter)       | 指定したメディア形式で結果を返します。|[`/users?$format=json`][format-example]
| [$orderby](#orderby-parameter)     | 結果を並べます。|[`/users?$orderby=displayName desc`][orderby-example]
| [$search](#search-parameter)       | 検索条件に基づいて結果を返します。現在、**messages** と **person** のコレクションでサポートされています。|[`/me/messages?$search=pizza`][search-example]
| [$select](#select-parameter)       | プロパティ (列) をフィルターします。|[`/users?$select=givenName,surname`][select-example]
| [$skip](#skip-parameter)           | 結果セットにインデックスを作成します。また一部の API でページングを実装するために使用されており、`$top` と組み合わせて結果を手動でページングすることもできます。 | [`/me/messages?$skip=11`][skip-example]
| [$skipToken](#skiptoken-parameter) | 複数ページにわたる結果セットから、結果の次のページを取得します。(一部の API では代わりに `$skip` を使用します。) | `/users?$skiptoken=X%274453707402000100000017...`|
| [$top](#top-parameter)             | 結果のページ サイズを設定します。 |[`/users?$top=2`][top-example]



これらのパラメーターは、[OData V4 クエリ言語][odata-query]と互換性があります。 すべての Microsoft Graph API で全部のパラメーターがサポートされているわけではなく、`v1.0` エンドポイントと `beta` エンドポイントの間でサポートが大幅に異なる場合があります。 

> **注:** `beta` と `v1.0` エンドポイントでは、`$` プレフィックスはオプションです。 たとえば、`$filter` の代わりに、`filter` を使用しても同じです。 

## <a name="encoding-query-parameters"></a>クエリ パラメーターのエンコード

クエリ パラメーターの値はパーセント エンコードされる必要があります。 これを行ううえで役立つ HTTP クライアント、ブラウザー、およびツールが多くあります ([Graph エクスプローラー][graph-explorer]など)。 クエリが失敗する場合、クエリ パラメーターの値が適切にエンコードされていないことがその原因の 1 つとして考えられます。

エンコードされていない URL は、次のようになります。

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

正しくエンコードされている URL は、次のようになります。

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## <a name="count-parameter"></a>count パラメーター

`$count` クエリ パラメーターを使用し、Microsoft Graph から返されるデータ値のページにコレクション内の項目数の合計を含めます。 

たとえば、次のような要求では、現在のユーザーの **contact** コレクションと、`@odata.count` プロパティ内の **contact** コレクションのアイテム数の両方が返されます。

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[Graph エクスプローラーで試す](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


>**注:** `$count` は、[user](/graph/api/resources/user?view=graph-rest-1.0) や [group](/graph/api/resources/group?view=graph-rest-1.0) のコレクションのような、[directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) から派生したリソースのコレクションに対してはサポートされていません。

## <a name="expand-parameter"></a>expand パラメーター

Microsoft Graph リソースの多くは、宣言されているリソースのプロパティと、他のリソースとのリレーションシップの両方を公開します。 これらのリレーションシップは、参照プロパティまたはナビゲーション プロパティとも呼ばれ、1 つのリソースまたはリソースのコレクションのいずれかを参照することができます。 たとえば、ユーザーのメール フォルダー、マネージャー、直属の部下は、すべてリレーションシップとして公開されます。 

通常、単一の要求では、リソースの複数のプロパティ、またはリソースのリレーションシップの 1 つのいずれかに対してクエリを実行できますが、両方は行えません。`$expand` クエリ文字列パラメーターを使用して、展開されているリソース、または単一のリレーションシップ (ナビゲーション プロパティ) で参照されているコレクションを結果に含めることができます。

次の例では、ドライブ内のトップレベルの子項目と共に、ルート ドライブ情報を取得します。

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[Graph エクスプローラーで試す](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

いくつかのリソース コレクションで、`$select` パラメーターを追加すれば、展開されたリソースで返されるプロパティを指定することもできます。次の使用例は前の例と同じクエリを実行しますが、[`$select`](#select-parameter) ステートメントを使用して、展開されている子項目に返されるプロパティを **id** プロパティと **name** プロパティに限定します。

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

[Graph エクスプローラーで試す][expand-example]

> **注:** すべてのリレーションシップとリソースで、`$expand` クエリ パラメーターがサポートされているわけではありません。たとえば、ユーザーの **directReports**、**manager**、**memberOf** の各リレーションシップを展開できますが、その **events**、**messages**、**photo** のリレーションシップは展開できません。すべてのリソースまたはリレーションシップで、`$select` を使用して展開されたアイテムがサポートされているわけではありません。 
> 
> [ユーザー](/graph/api/resources/user?view=graph-rest-1.0)や[グループ](/graph/api/resources/group?view=graph-rest-1.0)のような、[directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) から派生した Azure AD リソースの場合、`$expand` は `beta` でのみサポートされており、通常は展開されているリレーションシップに対し最大 20 個のアイテムを返すことができます。

## <a name="filter-parameter"></a>filter パラメーター

`$filter` クエリ パラメーターを使用して、コレクションのサブセットのみを取得します。 

たとえば、表示名が「J」という文字で始まるユーザーを検索するには、`startswith` を使用します。

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

[Graph エクスプローラーで試す][filter-example]

`$filter` 演算子のサポートは、お使いの Microsoft Graph API によって異なります。 通常、次の論理演算子がサポートされています。 

- 等しい (`eq`)
- 等しくない (`ne`)
- より大きい (`gt`)
- 以上 (`ge`)
- より小さい (`lt`)、以下 (`le`)
- AND (`and`)
- OR (`or`)
- NOT (`not`)
 
`startswith` 文字列の演算子はたいていサポートされています。 `any` ラムダ演算子は、一部の API でサポートされています。 いくつかの使用例について、次の表を参照してください。 `$filter` 構文の詳細については、「[OData プロトコル][odata-filter]」を参照してください。  

次の表では、`$filter` クエリ パラメーター使用例を示します。

> **注:** 例をクリックして [Graph エクスプローラー][graph-explorer]で試行します。

| 説明 | 例
|:------------|:--------|
| 複数のプロパティ間で Mary という名前を持つユーザーを検索します。 | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) 
| 2017 年 7 月 1 日以降に開始する、サインイン ユーザーのイベントすべてを取得します。 | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) 
| サインイン ユーザーが受信した特定のアドレスからの電子メールすべてを取得します。 | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) 
| 2017 年 4 月にサインイン ユーザーが受信した電子メールすべてを取得します。 | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) 
| サインイン ユーザーの受信トレイから未読メールをすべて取得します。 | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) 
| 組織内のすべての Office 365 グループの一覧 | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) 

> **注:** Azure AD リソースでは、次の `$filter` 演算子はサポートされていません: `ne`、`gt`、`ge`、`lt`、`le`、`not`。Microsoft Graph リソースでは現在、`contains` 文字列の演算子はサポートされていません。

## <a name="format-parameter"></a>format パラメーター

`$format` クエリ パラメーターを使用して、Microsoft Graph から返される項目のメディア形式を指定します。

たとえば、次の要求では組織のユーザーが JSON 形式で返されます。

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

[Graph エクスプローラーで試す][format-example]

> **注:**`$format` クエリ パラメーターは、さまざまな形式 (atom、xml、json など) をサポートしていますが、結果がすべての形式で返されるわけではありません。

## <a name="orderby-parameter"></a>orderby パラメーター

`$orderby` クエリ パラメーターを使用して、Microsof Graph から返される項目の並べ替え順序を指定します。

たとえば、次の要求では組織のユーザーが表示名順で返されます。

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
[Graph エクスプローラーで試す][orderby-example]

複合型のエンティティでも並べ替えができます。次の要求では、メッセージを取得し、それらを **emailAddress** という複合型である **from** プロパティの **address** フィールドで並べ替えます。

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[Graph エクスプローラーで試す](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

昇順または降順で結果を並べ替えるには、`asc` または `desc` のいずれかをスペースで区切ってフィールド名の後に追加します。たとえば `?$orderby=name%20desc` のようにします。

一部の API では、複数のプロパティの結果を並べ替えることができます。 たとえば、次のような要求ではユーザーの受信トレイ内のメッセージを、最初は送信者の名前で降順に並べ替え (Z から A)、次に件名で昇順 (既定) に並べ替えます。

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

[Graph エクスプローラーで試す](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)

$filter を指定した場合は、サーバーで結果の並べ替え順序が考慮されます。 `$orderby` と `$filter` の両方を使用する場合、サーバーでは常に `$filter` の結果の並べ替え順序が考慮されるため、`$filter` 内のプロパティを他のプロパティよりも先に `$orderby` 内に配置して、`$filter` パラメーターに現れる順序で並べる必要があります。 

次の例は、**Subject** と **Importance** の両方のプロパティでフィルター処理されてから、**Subject**、**Importance**、**receivedDateTime** の各プロパティで降順で並べ替えられたクエリを示しています。

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```

[Graph エクスプローラーで試す](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=subject%20eq%20%27welcome%27%20and%20importance%20eq%20%27normal%27%20&$orderby=subject,importance,receivedDateTime%20desc&method=GET&version=v1.0)

 > **注:** [ユーザー](/graph/api/resources/user?view=graph-rest-1.0)や[グループ](/graph/api/resources/group?view=graph-rest-1.0)のような、[directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) から派生した Azure AD リソースの場合、`$orderby` 式と `$filter` 式を結合することはできません。 

## <a name="search-parameter"></a>search パラメーター

`$search` クエリ パラメーターを使用して、要求の結果を検索条件と一致するものに制限します。

> **注:** 現在の検索対象は、[メッセージ](/graph/api/resources/message?view=graph-rest-1.0) コレクションと[人物](/graph/api/resources/person?view=graph-rest-1.0)コレクション**だけ**です。`$search` 要求は最大 250 まで結果を返します。検索要求では [`$filter`](#filter-parameter) も [`$orderby`](#orderby-parameter) も使用できません。

### <a name="using-search-on-message-collections"></a>メッセージ コレクションで $search を使用する

特定のメッセージ プロパティの値に基づいてメッセージを検索することができます。 検索結果は、メッセージが送信された日時で並べ替えられます。

メッセージで検索を行うときに、特定のメッセージ プロパティを指定せずに値のみを指定した場合、検索は既定の検索プロパティである **from**、**subject**、**body** に基づいて行われます。

次の例は、サインイン中のユーザーの受信トレイにあるメッセージのうち、既定の 3 つの検索プロパティのいずれかに "pizza" が含まれるメッセージをすべて返します。

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

[Graph エクスプローラーで試す][search-example]

また、キーワード クエリ言語 (KQL) 構文で認識される、以下の表のメッセージ プロパティ名を指定して、メッセージの検索をすることもできます。 これらのプロパティ名は Microsoft Graph の **message** エンティティで定義したプロパティです。 Outlook や他の Office 365 アプリケーション (SharePoint など) では KQL 構文をサポートしており、データ ストアの共通探索ドメインの利便性が向上します。


| 検索可能な電子メール プロパティ                | 説明 | 例 
|:-------------------------|:------------|:---------|
| **attachment**           | 電子メール メッセージに添付されているファイルの名前。|[`me/messages?$search="attachment:api-catalog.md"`][search-att-example]
| **bcc**           | SMTP アドレス、表示名、エイリアスとして指定されている、電子メール メッセージの **bcc** フィールド。|[`me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`][search-bcc-example]
| **body**           | 電子メール メッセージの本文。|[`me/messages?$search="body:excitement"`][search-body-example]
| **cc**           | SMTP アドレス、表示名、エイリアスとして指定されている、電子メール メッセージの **cc** フィールド。|[`me/messages?$search="cc:danas"&$select=subject,ccRecipients`][search-cc-example]
| **from**           | SMTP アドレス、表示名、エイリアスとして指定されている、電子メール メッセージの送信者。|[`me/messages?$search="from:randiw"&$select=subject,from`][search-from-example]
| **hasAttachment** | 電子メール メッセージに添付ファイルがあり、そのファイルがインラインの添付ファイルでない場合は true、そうでない場合は false。 |[`me/messages?$search="hasAttachments=true"`][search-from-example]
| **importance**           | 送信者がメッセージを送信するときに指定できる電子メール メッセージの重要度。 使用可能な値: `low`、`medium`、`high`。|[`me/messages?$search="importance:high"&$select=subject,importance`][search-imp-example]
| **kind**           | メッセージの種類。 使用可能な値: `contacts`、`docs`、`email`、`faxes`、`im`、`journals`、`meetings`、`notes`、`posts`、`rssfeeds`、`tasks`、`voicemail`。|[`me/messages?$search="kind:voicemail"`][search-kind-example]
| **participants**           | SMTP アドレス、表示名、エイリアスとして指定されている、電子メール メッセージの **from**、**to**、**cc**、**bcc** フィールド。|[`me/messages?$search="participants:danas"`][search-part-example]
| **received**           | 電子メール メッセージが受信者によって受信された日付。|[`me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`][search-rcvd-example]
| **recipients**           | SMTP アドレス、表示名、エイリアスとして指定されている、電子メール メッセージの **to**、**cc**、**bcc** フィールド。|[`me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients`][search-rcpts-example]
| **sent**           | 送信者によって電子メール メッセージが送信された日付。|[`me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`][search-sent-example]
| **size**           | アイテムのサイズ (バイト数)。|[`me/messages?$search="size:1..500000"`][search-size-example]
| **subject**           | 電子メール メッセージの件名行に含まれるテキスト。 .|[`me/messages?$search="subject:has"&$select=subject`][search-sbj-example]
| **to**           | SMTP アドレス、表示名、エイリアスとして指定されている、電子メール メッセージの **to** フィールド。|[`me/messages?$search="to:randiw"&$select=subject,toRecipients`][search-to-example]


検索可能な電子メール プロパティ、KQL 構文、サポートされている演算子、検索のヒントなどの詳細については、次の記事を参照してください。

- [Exchange の検索可能なプロパティ](https://docs.microsoft.com/ja-JP/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange)。

- [キーワード クエリ言語 (KQL) 構文のリファレンス](https://docs.microsoft.com/ja-JP/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- 
  [Exchange 2016 におけるインプレースの電子情報開示のためのメッセージ プロパティと検索演算子](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)

### <a name="using-search-on-person-collections"></a>人物コレクションで $search を使用する

Microsoft Graph People API を使用してユーザーに最も関連のある人物を取得できます。関連性は、ユーザーのコミュニケーションとコラボレーション パターン、およびビジネスのリレーションシップによって決定されます。People API では、`$search` クエリ パラメーターがサポートされています。

[person](/graph/api/resources/person?view=graph-rest-1.0) リソースの **displayName** プロパティと **emailAddress** プロパティの両方で人物の検索を行います。

次の要求は、サインイン ユーザーの **people** コレクションに含まれる各ユーザーの **displayName** プロパティと **emailAddress** プロパティで、「Irene McGowen」という名前の人物を検索します。 「Irene McGowan」という名前の人物がサインインしているユーザーに関連するため、「Irene McGowan」の情報が返されます。

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

次の例は応答を示しています。 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
           "id": "C0BD1BA1-A84E-4796-9C65-F8A0293741D1",
           "displayName": "Irene McGowan",
           "givenName": "Irene",
           "surname": "McGowan",
           "birthday": "",
           "personNotes": "",
           "isFavorite": false,
           "jobTitle": "Auditor",
           "companyName": null,
           "yomiCompany": "",
           "department": "Finance",
           "officeLocation": "12/1110",
           "profession": "",
           "userPrincipalName": "irenem@contoso.onmicrosoft.com",
           "imAddress": "sip:irenem@contoso.onmicrosoft.com",
           "scoredEmailAddresses": [
               {
                   "address": "irenem@contoso.onmicrosoft.com",
                   "relevanceScore": -16.446060612802224
               }
           ],
           "phones": [
               {
                   "type": "Business",
                   "number": "+1 412 555 0109"
               }
           ],
           "postalAddresses": [],
           "websites": [],
           "personType": {
               "class": "Person",
               "subclass": "OrganizationUser"
           }
       }
   ]
}
```

People API の詳細については、「[関係する人の情報を取得する](./people-example.md#search-people)」を参照してください。  

## <a name="select-parameter"></a>select パラメーター

`$select` クエリ パラメーターを使用して、個別リソースまたはリソースのコレクションの既定値とは異なるプロパティのセットを返します。 $Select で、既定のプロパティのサブセットまたはスーパーセットを指定できます。

たとえば、サインイン ユーザーのメッセージを取得するとき、**from** プロパティと **subject** プロパティだけを返すよう指定できます。

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

[Graph エクスプローラーで試す][select-example]

> **重要:** 通常は、`$select` を使用して、クエリから返されるプロパティをお使いのアプリで必要なものだけに制限することをお勧めします。 これは特に、クエリが大きな結果セットを返す可能性がある場合に該当します。 行ごとに返されるプロパティを制限すれば、ネットワークの負荷を軽減し、アプリのパフォーマンスを向上させることができます。
>
> `v1.0`では、[ユーザー](/graph/api/resources/user?view=graph-rest-1.0)と[グループ](/graph/api/resources/group?view=graph-rest-1.0)のような、[directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) から派生した一部の Azure AD リソースは、読み取り時に制限された既定値のプロパティ サブセットを返します。既定のセット以外のプロパティを返すには、これらのリソースに対して `$select` を使用する必要があります。  

## <a name="skip-parameter"></a>skip パラメーター

コレクションを開始するときにスキップする項目数を設定するには、`$skip` クエリ パラメーターを使用します。たとえば、次の要求はユーザーのイベントを、コレクション内の 21 番目以降のイベントから作成日順で返します。

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
[Graph エクスプローラーで試す][skip-example]

> **注:** Outlook のメールやカレンダーなど、いくつかの Microsoft Graph API (**message**、**event**、**calendar**) は、`$skip` を使用してページングを実装します。 クエリの結果が複数ページにまたがる場合、これらの API は `@odata:nextLink` プロパティと共に `$skip` パラメーターが含まれる URL を返します。 この URL を使用して、結果の次のページに戻れます。 詳細については、「[ページング](./paging.md)」を参照してください。

## <a name="skiptoken-parameter"></a>skipToken パラメーター

要求の中には、サーバー側のページングを使用したり、応答におけるページ サイズを限定するために [`$top`](#top-parameter) パラメーターを使用したりすることによって、複数のデータ ページを返すものがあります。Microsoft Graph API の多くは、`skipToken` クエリ パラメーターを使用して、結果の後続のページを参照します。`$skiptoken` パラメーターは、結果の次のページを参照する不透明トークンを含んでおり、応答の `@odata.nextLink` プロパティで指定される URL で返されます。詳細については、「[ページング](./paging.md)」を参照してください。


## <a name="top-parameter"></a>top パラメーター

`$top` クエリ パラメーターを使用して、結果セットのページ サイズを指定します。 

結果セットにさらに項目が残っている場合、応答本文に `@odata.nextLink` パラメーターが含まれます。 このパラメーターには、結果の次のページを取得するために使用できる URL が含まれています。 詳細については、「[ページング](./paging.md)」を参照してください。 

たとえば、次の要求はユーザーのメールボックスの最初の 5 つのメッセージを返します。

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

[Graph エクスプローラーで試す][top-example]


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

ただし、要求で指定されたクエリ パラメーターが警告なしで失敗する可能性があるため、注意が必要です。 これは、クエリ パラメーターがサポートされていない場合や、クエリ パラメーターの組み合わせがサポートされていない場合に起こり得ます。 その場合、要求によって返されたデータを調べ、指定したクエリ パラメーターに期待どおりの効果があったかどうかを確認する必要があります。 

[graph-explorer]: https://developer.microsoft.com/graph/graph-explorer
[odata-filter]: https://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: https://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
[count-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0
[expand-example]: https://developer.microsoft.com/graph/graph-explorer?request=groups?$expand=members&method=GET&version=v1.0
[filter-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0
[format-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$format=json&method=GET&version=v1.0
[orderby-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0
[search-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0
[select-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0
[skip-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0
[top-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0

[search-att-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22attachment%3Aapi-catalog%2Emd%22&method=GET&version=v1.0
[search-bcc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22bcc%3Asamanthab%40contoso%2Ecom%22%26$select=subject,bccRecipients&method=GET&version=v1.0
[search-body-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22body%3Aexcitement%22&method=GET&version=v1.0
[search-cc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22cc%3Adanas%22%26$select=subject,ccRecipients&method=GET&version=v1.0
[search-from-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22from%3Arandiw%22%26$select=subject,from&method=GET&version=v1.0
[search-hasatt-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22hasAttachments=true%22&method=GET&version=v1.0
[search-imp-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22importance%3Ahigh%22%26$select=subject,importance&method=GET&version=v1.0
[search-kind-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22kind%3Avoicemail%22&method=GET&version=v1.0
[search-part-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22participants%3Adanas%22&method=GET&version=v1.0

[search-rcvd-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22received%3A07/23/2018%22%26$select=subject,receivedDateTime&method=GET&version=v1.0

[search-rcpts-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22recipients%3Arandiw%22%26$select=subject,toRecipients,ccRecipients,bccRecipients&method=GET&version=v1.0
[search-sent-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22sent%3A07/23/2018%22%26$select=subject,sentDateTime&method=GET&version=v1.0
[search-size-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22size%3A1%2E%2E500000%22&method=GET&version=v1.0

[search-sbj-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22subject%3Ahas%22%26$select=subject&method=GET&version=v1.
[search-to-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22to%3Arandiw%22%26$select=subject,toRecipients&method=GET&version=v1.0

