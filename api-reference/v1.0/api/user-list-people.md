---
title: ユーザーを一覧表示する
description: ユーザーとの関連 (ユーザーのコミュニケーションとコラボレーション パターン、およびビジネスのリレーションシップによって決まる) によって配列された人物オブジェクトのコレクションを取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 4edbb397436be86bb305e1695566c7d2a4bb7c07
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728980"
---
# <a name="list-people"></a>ユーザーを一覧表示する

[ユーザー](../resources/user.md)との関連 (ユーザーのコミュニケーションとコラボレーション パターン、およびビジネスのリレーションシップによって決まる) によって配列された[人物](../resources/person.md)オブジェクトのコレクションを取得します。

この情報は、People API 経由で取得できます。例については、「[例](#examples)」セクションと記事「[人の関連情報を取得する](/graph/people-example)」を参照してください。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | People.Read、People.Read.All    |
|委任 (個人用 Microsoft アカウント) | People.Read    |
|アプリケーション | People.Read.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドでは、「[ユーザーの関連情報を取得する](/graph/people-example)」の記事に示す例のように、[OData クエリ パラメーター](/graph/query-parameters)を使用して応答をカスタマイズすることができます。

|名前|値|説明|
|:---------------|:--------|:-------|
|$filter|string|応答を、指定した条件に等しいレコードを持つ人物のみに制限します。|
|$orderby|string|既定では、応答に含まれる人物は、クエリとの関連性で並べ替えられます。 応答に含まれる人物の順序は、*$orderby* パラメーターを使用することで変更できます。|
|$search|string|名またはエイリアスで人物を検索します。 ファジー マッチをサポートします。 パラメーターは、サインインしたユーザーの関連人物を検索するためにのみ機能し、他のユーザーに関連する人物を検索するためには機能しません。 その人とのメール会話から抽出されたトピックに基づいて人を見つける `topic` キーワードもサポートします。 情報と例については、[関係者の情報を取得する](/graph/people-example#perform-a-fuzzy-search)の*あいまい検索の実行*セクションを参照してください。 |
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

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [person](../resources/person.md) オブジェクトのコレクションを返します。応答には、1 つの person オブジェクトまたは person オブジェクトのコレクションを含めることができます。

## <a name="examples"></a>例

#### <a name="request"></a>要求

要求の例を次に示します。


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/people
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-person-collection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-person-collection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-person-collection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-person-collection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>応答

応答の例を次に示します。

<!-- {
  "blockType": "response",
  "name": "get_person_collection",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1370

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
            "jobTitle": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "userPrincipalName": "",
            "imAddress": null,
            "scoredEmailAddresses": [
                {
                    "address": "Marketing@contoso.com",
                    "relevanceScore": 30.0
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Group",
                "subclass": "UnifiedGroup"
            }
        },
        {
            "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
            "displayName": "Isaiah Langer",
            "givenName": "Isaiah",
            "surname": "Langer",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "userPrincipalName": "IsaiahL@contoso.com",
            "imAddress": "sip:isaiahl@contoso.com",
            "scoredEmailAddresses": [
                {
                    "address": "IsaiahL@contoso.com",
                    "relevanceScore": 20.0
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
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        }
    ]
}
```

他の例については、「[関係する人の情報を取得する](/graph/people-example)」を参照してください。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
