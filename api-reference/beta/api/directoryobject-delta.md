---
title: 'directoryObject: delta'
description: 単一のデルタクエリで、次の種類の新規作成、更新、または削除されたディレクトリオブジェクトを取得します。ユーザー、グループ、組織の連絡先。 詳細は変更の追跡をご覧ください。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cebf8676b1c81a41ed77f259fb3b3775f8fafdef
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319567"
---
# <a name="directoryobject-delta"></a>directoryObject: delta

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

単一のデルタクエリで、次の種類の新規作成、更新、または削除されたディレクトリオブジェクトを取得します。[ユーザー](../resources/user.md)、[グループ](../resources/group.md)、[組織の連絡先](../resources/orgcontact.md)。 詳細は.、[変更の追跡](/graph/delta-query-overview)をご覧ください。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.Read.All、Directory.AccessAsUser.All  |
|委任 (個人用 Microsoft アカウント) | サポートされていません。  |
|アプリケーション | Directory.Read.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

変更の追跡を開始するには、directoryObjects リソースにデルタ関数を含む要求を行います。

<!-- { "blockType": "ignored" } -->

```http
GET /directoryObjects/delta
```

## <a name="query-parameters"></a>クエリ パラメーター

変更の追跡では、1回以上の**デルタ**関数呼び出しが発生します。 任意のクエリ パラメーター (`$deltatoken` と`$skiptoken`以外) を使用する場合は、最初の**デルタ**要求でこれを指定する必要があります。 Microsoft Graph は、応答で提供される `nextLink` または `deltaLink` の URL のトークン部分に指定したパラメーターを自動的にエンコードします。

必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。

その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。

| クエリ パラメーター | 種類 |説明|
|:---------------|:--------|:----------|
| $deltatoken | string | 同じユーザー コレクションの前の**デルタ**関数の `deltaLink` URL で[状態トークン](/graph/delta-query-overview)が返され、変更追跡のその回が完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。|
| $skiptoken | string | 前の**デルタ**関数の `nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じユーザー コレクションで追跡されるその他の変更があることを示します。 |

### <a name="odata-query-parameters"></a>OData クエリ パラメーター

このメソッドは、応答をカスタマイズするためのオプショナルの OData クエリ パラメーターをサポートします。

- 特別な`isOf`演算子`$filter`と共にを使用して、directoryobject から派生した型のサブセットをフィルター処理できます。
  - を使用して複数の式`or`を組み合わせることができます。これにより、1つのデルタクエリで複数の種類を追跡できます。 詳細については、 [3 番目の例](#request-3)を参照してください。

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 説明|
|:---------------|:----------|
| Authorization  | Bearer &lt;token&gt;|
| Content-Type  | application/json |
| Prefer | return=minimal. <br><br>このヘッダーを指定する要求を使用すると、`deltaLink` は、最後のラウンド以降に変更されたオブジェクトのプロパティのみを返します。 省略可能です。 |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

### <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/directoryobject.md) コレクション オブジェクトを返します。 応答には`nextLink` URLまたは`deltaLink` URLも含まれます。

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


> **注意:** この動作では、応答を見ても、プロパティが変化しているかどうかを判断することはできません。 また、デルタ応答は、すべてのプロパティ値を含むため、サイズが大きくなる傾向があります。

#### <a name="alternative-return-only-the-changed-properties"></a>代替案：変更されたプロパティのみを返す

オプションのリクエストヘッダを追加すると、- `prefer:return=minimal` - 次のようになります:

- プロパティを変更した場合は、応答には新しい値が含まれます。 これには、null 値に設定されているプロパティが含まれます。
- プロパティが変更されていない場合、そのプロパティは応答にまったく含まれません。 (既定の動作と異なる)

> **注意:** ヘッダーは、デルタサイクルのどの時点でも `deltaLink`要求に追加できます。 ヘッダーは応答に含まれる一連のプロパティにのみ影響し、デルタクエリの実行方法には影響しません。

## <a name="example"></a>例

### <a name="request-1"></a>要求 1

要求の例を次に示します。 `$select`パラメータがないため、デフォルトのプロパティセットが追跡されて返されます。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directory_object_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directory-object-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directory-object-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directory-object-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directory-object-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-1"></a>応答 1

以下は、クエリ初期化から取得した`deltaLink` を使用した場合の応答の例です。 フィルター `isOf`は使用されていないので、directoryobject から派生したすべての型が返されます。

>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 実際の呼び出しではすべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "city": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "createdDateTime": null,
      "department": null,
      "displayName": "John Smith",
      "givenName": null,
      "jobTitle": null
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp"
    },
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "8f301319-4b4e-493f-8067-bce1dec76e7a",
      "businessPhones": ["string"],
      "city": "string",
      "companyName": "string",
      "country": "string",
      "department": "string",
      "displayName": "string",
      "givenName": "string",      
      "jobTitle": "string"
    }
  ]
}
```

### <a name="request-2"></a>要求 2

次の例は、代替の最小応答動作の使用法を示しています。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryObject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
Prefer: return=minimal
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-2"></a>応答 2

以下は、クエリ初期化から取得した`deltaLink` を使用した場合の応答の例です。 メモ実際に変更されたプロパティのみが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "displayName": "John Smith"
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "description": null,
      "displayName": "testgp"
    },
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "8f301319-4b4e-493f-8067-bce1dec76e7a",
      "businessPhones": "12345"
    }
  ]
}
```

### <a name="request-3"></a>要求 3

次の例では、 `isOf`演算子を使用して、ユーザーエンティティとグループエンティティのみを除外する最初の要求を示しています。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta?$filter=isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-3"></a>応答 3

以下は、クエリ初期化から取得した`deltaLink` を使用した場合の応答の例です。 ユーザーオブジェクトとグループオブジェクトのみが返されることに注意してください。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "city": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "createdDateTime": null,
      "department": null,
      "displayName": "John Smith",
      "givenName": null,
      "jobTitle": null
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp"
    }
  ]
}
```

- [デルタクエリを使用してMicrosoft Graphデータの変更を追跡します](/graph/delta-query-overview)。
- [ユーザーの増分変更を取得します](/graph/delta-query-users)。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
