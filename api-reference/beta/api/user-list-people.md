---
title: ユーザーを一覧表示する
description: ユーザーのコミュニケーションとコラボレーションパターン、およびビジネス上の関係によって決定される、ユーザーに対して関連性のある人物が注文した人物オブジェクトのリストを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: de07eaa4b3601c91ace9894e55bd4357fbb23881
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637193"
---
# <a name="list-people"></a>ユーザーを一覧表示する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーのコミュニケーションとコラボレーションパターン、およびビジネス上の関係によって決定される、[ユーザー](../resources/user.md)に対して関連性のある人物が注文した[人物](../resources/person.md)オブジェクトのリストを取得します。

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

このメソッドは、応答をカスタマイズするために、次の OData クエリパラメーターをサポートします。

|名前|値|説明|
|:---------------|:--------|:-------|
|$filter|string|応答を、指定した条件に等しいレコードを持つ人物のみに制限します。|
|$orderby|string|既定では、応答に含まれる人物は、クエリとの関連性で並べ替えられます。 応答に含まれる人物の順序は、*$orderby* パラメーターを使用することで変更できます。|
|$search|string|名またはエイリアスで人物を検索します。 ファジー マッチをサポートします。 パラメーターは、サインインしたユーザーの関連人物を検索するためにのみ機能し、他のユーザーに関連する人物を検索するためには機能しません。 その人とのメール会話から抽出されたトピックに基づいて人を見つける `topic` キーワードもサポートします。 情報と例については、[関係者の情報を取得する](/graph/people-example#perform-a-fuzzy-search)の*あいまい検索の実行*セクションを参照してください。|
|$select|string|応答に含めるプロパティを示すコンマ区切りのリスト。最適なパフォーマンスを得るには、必要なプロパティのサブセットのみを選択します。|
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

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[person](../resources/person.md)オブジェクトのコレクションを返します。

## <a name="examples"></a>例

### <a name="browse"></a>参照

このセクションの要求は、コミュニケーション、コラボレーション、およびビジネスのリレーションシップに基づいて`/me`、サインインしているユーザーに最も関連のある人物を取得します ()。

既定では、応答ごとに 10 件のレコードが返されます。ただし、$top パラメーターを使用することで、*これを変更*できます。 これらの要求には、ユーザーの読み取りアクセス許可が必要です。

#### <a name="request"></a>要求

既定の要求の例を次に示します。
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
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/get_person_collection_beta-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_person_collection_beta-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

#### <a name="requesting-a-subsequent-page-of-people"></a>人物の続きのページの要求

最初の応答に関連のある人物のリストを完全に含められない場合は、追加の情報ページを要求するために、*$top* と *$skip* を使用して 2 番目の要求を行うことができます。前の要求に追加情報が含まれている場合は、次の要求でサーバーから人物についての後続ページを取得します。

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a>応答の並べ替え

既定では、応答に含まれる人物は、クエリとの関連性で並べ替えられます。 応答に含まれる人物の順序は、*$orderby* パラメーターを使用することで変更できます。 このクエリでは、自分に最も関連のある人物を選択し、その人物を表示名で並べ替えてから、最初の 10 人の人物を並べ替え済みのリストで返します。

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a>返される人物の数と返されるフィールドの変更

応答で返される人物の数は、*$top* パラメーターを設定することで変更できます。

次の例では、最も関連のある`/me`1000 ユーザーを要求します。 また、この要求では、人物の表示名のみを要求することで、サーバーから返されるデータの量も制限しています。

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

次のクエリは、ソース "Directory" を持つユーザーに対する応答を制限します。

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a>フィルター処理された応答で返されるフィールドを選択する

*$select* パラメーターと *$filter* パラメーターを組み合わせることで、ユーザーに関連のある人物のカスタム リストを作成し、アプリケーションで必要になるフィールドのみを取得できます。

次に示す例では、指定した名前と等しい表示名を持つ人物の *DisplayName* と *EmailAddress* を取得します。 この例では、表示名が "Nestor Kellum" と等しい人物のみが返されます。

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a>人物の検索

このセクションの要求は、サインインしているユーザーに最も関連のある人物を`/me`取得することもできます ()。 検索要求には、ユーザーの読み取りアクセス許可が必要です。

#### <a name="using-search-to-select-people"></a>検索による人物の選択

*$search* パラメーターを使用して、特定の条件セットを満たす人物を選びます。

次の検索クエリは、GivenName また`/me`は姓が "j" という文字で始まる人物を返します。

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a>検索による関連するトピックの指定

次の要求では、名前`/me`に "ma" が含まれていて、"機能の計画" と関連付けられている人物を返します。

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a>あいまい検索の実行

次に示す要求では、"Hermaini Hall" という名前の人物について検索を実行します。 サインインしているユーザーに関連する "Herminia Hull" という名前の人物が存在するため、"Herminia Hull" の情報が返されます。

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a>関連する人

次の要求は、ユーザーの組織内の他のユーザーに最も関連のある人物を取得します。 この要求には、ユーザーに対してすべてのアクセス許可が必要です。 この例では、Nestor Kellum の関連する人物が表示されます。

```http
GET https://graph.microsoft.com/beta/users('nestork@contoso.com')/people/
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-people.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-people.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
