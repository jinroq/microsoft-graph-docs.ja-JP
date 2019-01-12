---
title: ユーザーを一覧表示する
description: Person オブジェクトのユーザーの通信とコラボレーションのパターンとビジネスの関係によって決定されると、ユーザーに関連性の順のリストを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4233c0bc4015525bb474499366c084483ceaefe7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925043"
---
# <a name="list-people"></a>ユーザーを一覧表示する

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[Person](../resources/person.md)オブジェクトの順に、[ユーザー](../resources/user.md)ユーザーの通信とコラボレーションのパターンとビジネスの関係によって決定される関連性についての一覧を取得します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | People.Read    |
|委任 (個人用 Microsoft アカウント) | People.Read    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするためには、次の OData クエリ パラメーターをサポートします。

|名前|値|説明|
|:---------------|:--------|:-------|
|$filter|文字列|応答を、指定した条件に等しいレコードを持つ人物のみに制限します。|
|$orderby|文字列|既定では、応答に含まれる人物は、クエリとの関連性で並べ替えられます。 応答に含まれる人物の順序は、*$orderby* パラメーターを使用することで変更できます。|
|$search|string|名またはエイリアスで人物を検索します。 ファジー マッチをサポートします。 パラメーターだけが、他のユーザーに関連する人の検索ではなく、サインインしているユーザーの関連するユーザーを検索します。 サポートしており、`topic`その人と電子メールのやり取りなどから抽出された項目に基づいて、ユーザーを検索するキーワードです。 例については、[人の関連情報を取得](/graph/people-example#perform-a-fuzzy-search)することで*あいまい検索を実行する*セクションを参照してください。|
|$select|文字列|応答に含めるプロパティを示すコンマ区切りのリスト。最適なパフォーマンスを得るには、必要なプロパティのサブセットのみを選択します。|
|$skip|int|最初の n 個の結果をスキップします。これはページングに役立ちます。これは *$search* の使用時にはサポートされません。|
|$top|int|返される結果の数。|

## <a name="request-headers"></a>要求ヘッダー

| 名前      |説明|
|:----------|:----------|
| Authorization  | ベアラー {トークン}。必須。 |
| 承諾 | application/json |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本体で[ユーザー](../resources/person.md)オブジェクトのコレクションです。

## <a name="examples"></a>例

### <a name="browse"></a>参照

このセクションで要求がサインインしているユーザーに最も関連する人を取得 (`/me`)、通信、コラボレーション、および取引関係に基づく。

既定では、応答ごとに 10 件のレコードが返されます。ただし、$top パラメーターを使用することで、*これを変更*できます。 これらの要求には、People.Read アクセス許可が必要です。

#### <a name="request"></a>要求

次に、既定の要求の例を示します。
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```http
GET https://graph.microsoft.com/beta/me/people
```

#### <a name="response"></a>応答

応答の例を次に示します。
>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "name": "get_person_collection_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1326

{
    "value": [
        {
            "id": "33b43a5b-87d6-41ec-91f8-a2610048105f",
            "displayName": "Marketing",
            "givenName": null,
            "surname": null,
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "mailboxType": "GroupMailbox",
            "personType": "ModernGroup",
            "userPrincipalName": "",
            "emailAddresses": [
                {
                    "address": "Marketing@contoso.com",
                    "rank": 30
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        },
        {
            "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
            "displayName": "Isaiah Langer",
            "givenName": "Isaiah",
            "surname": "Langer",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "mailboxType": "Mailbox",
            "personType": "Person",
            "userPrincipalName": "IsaiahL@contoso.com",
            "emailAddresses": [
                {
                    "address": "IsaiahL@contoso.com",
                    "rank": 20
                }
            ],
            "phones": [
                {
                    "type": "business",
                    "number": "+1 918 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        }
    ]
}
```

#### <a name="requesting-a-subsequent-page-of-people"></a>人物の続きのページの要求

最初の応答に関連のある人物のリストを完全に含められない場合は、追加の情報ページを要求するために、*$top* と *$skip* を使用して 2 番目の要求を行うことができます。前の要求に追加情報が含まれている場合は、次の要求でサーバーから人物についての後続ページを取得します。

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a>応答の並べ替え

既定では、応答に含まれる人物は、クエリとの関連性で並べ替えられます。応答に含まれる人物の順序は、*$orderby* パラメーターを使用することで変更できます。このクエリでは、自分に最も関連のある人物を選択し、その人物を表示名で並べ替えてから、最初の 10 人の人物を並べ替え済みのリストで返します。

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a>返される人物の数と返されるフィールドの変更

応答で返される人物の数は、*$top* パラメーターを設定することで変更できます。

次の例の要求に最も関連する 1,000 人`/me`。 また、この要求では、人物の表示名のみを要求することで、サーバーから返されるデータの量も制限しています。

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a>返されるフィールドの選択

サーバーから返されるデータの量は、1 つ以上のフィールドを選択する *$select* パラメーターを使用することで制限できます。*@odata.id* フィールドは常に返されます。

次に示す例では、最も関連のある 10 人の人物の *DisplayName* と *EmailAddress* に応答を制限します。

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a>フィルターを使用した応答の制限

*$filter* パラメーターを使用すると、指定した条件に等しいレコードを持つ人物のみに応答を制限できます。

次のクエリは、ソースの [ディレクトリ] にしますユーザーへの応答を制限します。

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a>フィルター処理された応答で返されるフィールドを選ぶ

*$select* パラメーターと *$filter* パラメーターを組み合わせることで、ユーザーに関連のある人物のカスタム リストを作成し、アプリケーションで必要になるフィールドのみを取得できます。

次に示す例では、指定した名前と等しい表示名を持つ人物の *DisplayName* と *EmailAddress* を取得します。この例では、表示名が "Nestor Kellum" と等しい人物のみが返されます。

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a>人物の検索

このセクション内の要求も取得ユーザー サインイン中のユーザーに最も関連する (`/me`)。 検索要求には、People.Read アクセス許可が必要です。

#### <a name="using-search-to-select-people"></a>検索による人物の選択

*$search* パラメーターを使用して、特定の条件セットを満たす人物を選びます。

人を返すに関連する次の検索クエリ`/me`名または姓を持つが、文字"j"で始まります。

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a>検索による関連するトピックの指定

人を返すに関連する次のような要求`/me`名前持つにはには、"ma"と「機能は計画」との関連付けがある人が含まれています。

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a>あいまい検索の実行

次に示す要求では、"Hermaini Hall" という名前の人物について検索を実行します。 サインイン中のユーザーに関連の「Herminia の船体」という名前の人があるため、「Herminia 船体」の情報が返されます。

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a>関連する人

次のような要求では、ユーザーの組織で他のユーザーに最も関連するユーザーを取得します。 この要求には、People.Read.All のアクセス許可を User.ReadBasic.All が必要です。 この例では、Nestor Kellum の関連する人が表示されます。

```http
GET https://graph.microsoft.com/beta/users('nestork@contoso.com')/people/
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
