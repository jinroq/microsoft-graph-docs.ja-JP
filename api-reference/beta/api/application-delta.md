---
title: 'アプリケーション: デルタ'
description: リソースコレクション全体の完全な読み取りを実行せずに、新しく作成、更新、または削除されたアプリケーションを取得します。 詳細については、「デルタクエリの使用」を参照してください。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aa3f7f0a5d7b07a23cc75652e66b8ca519e24a22
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318776"
---
# <a name="application-delta"></a>アプリケーション: デルタ

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

リソースコレクション全体の完全な読み取りを実行せずに、新しく作成、更新、または削除されたアプリケーションを取得します。 詳細については、「[デルタクエリの使用](/graph/delta-query-overview)」を参照してください。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Application.ReadWrite.All、Directory.Read.All |

## <a name="http-request"></a>HTTP 要求

変更の追跡を開始するには、アプリケーションリソースにデルタ関数を含む要求を行います。 

<!-- { "blockType": "ignored" } -->
```http
GET /applications/delta
```

### <a name="query-parameters"></a>クエリ パラメーター

変更の追跡では、1回以上の**デルタ**関数呼び出しが発生します。 任意のクエリ パラメーター (`$deltatoken` と`$skiptoken`以外) を使用する場合は、最初の**デルタ**要求でこれを指定する必要があります。 Microsoft Graph は、応答で提供される `nextLink` または `deltaLink` の URL のトークン部分に指定したパラメーターを自動的にエンコードします。 必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。 その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。

| クエリ パラメーター      | 種類   |説明|
|:---------------|:--------|:----------|
| $deltatoken | string | 同じリソースコレクションに対する前`deltaLink`の**デルタ**関数呼び出しの URL で返された[状態トークン](/graph/delta-query-overview)。変更追跡のラウンドが終了したことを示します。 そのコレクションの次の`deltaLink`ラウンドの変更追跡の最初の要求で、このトークンを含む URL 全体を保存して適用します。|
| $skiptoken | string | 前の**デルタ**関数呼び出しの`nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じリソースコレクションに追跡すべき変更が他にもあることを示します。 |

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための OData クエリ パラメーターをサポートします。

- 任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。 

- `$filter` に対するサポートには制限があります。
  * サポートされ`$filter`ている唯一の式は、id: `$filter=id+eq+{value}`または`$filter=id+eq+{value1}+or+id+eq+{value2}`を使用して特定のリソースの変更を追跡することです。 指定できる id の数は、URL の最大の長さによって制限されます。


## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | Bearer &lt;token&gt;|
| Content-Type  | application/json |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

### <a name="response"></a>応答

成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[application](../resources/application.md) collection オブジェクトを返します。 応答には、nextLink URL または deltaLink URL も含まれます。 

- URL が返される場合は、セッションに取得するデータの追加ページがあります。`nextLink` アプリケーションは`deltaLink` URL が応答に含まれるまで`nextLink` URLを使用して要求を続けます。

- URL が返される場合、返されるリソースの既存の状態に関するデータはありません。 今後のリソースの`deltaLink`変更点については、URL を永続化して使用してください。

参照先:</br>
- 詳細については、「[デルタ クエリの使用](/graph/delta-query-overview)」をご覧ください</br>
- 要求の例については、「[ユーザーに対する増分の変更の取得](/graph/delta-query-users)」をご覧ください。</br>

### <a name="example"></a>例
##### <a name="request"></a>要求

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_delta"
}-->
```http
GET https://graph.microsoft.com/beta/applications/delta
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>応答
注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#applications",
  "@odata.nextLink":"https://graph.microsoft.com/beta/applications/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
            "adminConsentDescription": "adminConsentDescription-value",
            "adminConsentDisplayName": "adminConsentDisplayName-value",
            "id": "id-value",
            "isEnabled": true,
            "type": "type-value",
            "userConsentDescription": "userConsentDescription-value",
            "userConsentDisplayName": "userConsentDisplayName-value",
            "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "application: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
