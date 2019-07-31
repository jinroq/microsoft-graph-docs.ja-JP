---
title: 'contactFolder: delta'
description: ユーザーのメールボックスで追加または削除された一連の連絡先フォルダーを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2e57ad54557f1478b4ac06fb8cafaa91343b8024
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943310"
---
# <a name="contactfolder-delta"></a>contactFolder: delta

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーのメールボックスで追加または削除された一連の連絡先フォルダーを取得します。

メールボックス内の連絡先フォルダーに対する**デルタ**関数の呼び出しと GET 要求とは似ていますが、[状態トークン](/graph/delta-query-overview)をこれらの呼び出しに適切に適用することにより、連絡先フォルダーの増分変更をクエリできる点が異なります。これにより、ユーザーの連絡先フォルダーのローカル ストアの保守と同期を行う際に、そのメールボックスの連絡先フォルダーすべてを毎回サーバーからフェッチする必要がなくなります。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Contacts.Read、Contacts.ReadWrite    |
|委任 (個人用 Microsoft アカウント) | Contacts.Read、Contacts.ReadWrite    |
|アプリケーション | Contacts.Read、Contacts.ReadWrite |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/delta
GET /users/<id>/contactFolders/delta
```

## <a name="query-parameters"></a>クエリ パラメーター

連絡先フォルダーの変更を追跡すると、一連の **デルタ**関数呼び出しが発生します。任意のクエリ パラメーター (`$deltatoken` と `$skiptoken` 以外) を使用する場合は、最初の**デルタ**要求でこれを指定する必要があります。Microsoft Graph は、応答で提供される `nextLink` のトークン部分 (`skiptoken` または `$deltatoken`) または `deltaLink` URL に指定したパラメーターを自動的にエンコードします。必要なクエリ パラメーターを前もって指定しておくだけで済みます。それ以降の要求では、前の応答で `nextLink` または `deltaLink` の URL に必要なパラメーターが既にエンコードされ、含まれているため、この URL をコピーして適用します。

| クエリ パラメーター      | 種類   |説明|
|:---------------|:--------|:----------|
| $deltatoken | string | 同じ連絡先フォルダー コレクションの前の**デルタ**関数呼び出しの `deltaLink` URL で[状態トークン](/graph/delta-query-overview)が返され、変更追跡のその回が完了したことを示します。このコレクションについて、このトークンを含む `deltaLink` URL 全体を、変更追跡の次の回の最初の要求に保存し、適用します。|
| $skiptoken | string | 前の**デルタ**関数呼び出しの `nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じ連絡先フォルダー コレクションに追跡すべき変更が他にもあることを示します。 |

### <a name="odata-query-parameters"></a>OData クエリ パラメーター

任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。 

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明 |
|:---------------|:----------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |
| Content-Type  | string  | application/json. Required. |
| Prefer | string  | odata.maxpagesize={x}.省略可能。 |

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [contactFolder](../resources/contactfolder.md) コレクション オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求
次の例に、**デルタ**関数呼び出しを 1 つ作成し、応答本文に含まれる連絡先フォルダーの最大数を 2 に制限する方法を示します。

メールボックスの連絡先フォルダー内の変更を追跡するには、1 つ以上の**デルタ**関数呼び出しを作成し、適切な状態トークンを使用して、前回のデルタ クエリ以降になされた一連の増分変更を取得します。 

メール フォルダー内のメッセージ変更を追跡するために状態トークンを使用する方法を示す同様の例については、次をご覧ください。[フォルダー内のメッセージへの増分の変更を取得する](/graph/delta-query-messages)。連絡先フォルダーの追跡とフォルダー内のメッセージの追跡の主な違いは、デルタ クエリ要求 URL のほかに、クエリ応答で **message** コレクションではなく **contactFolder** が返されることです。


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contactfolder_delta"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/delta

Prefer: odata.maxpagesize=2
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contactfolder-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contactfolder-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contactfolder-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>応答

要求が成功すると、応答には状態トークンが含まれます。これは、_skipToken_  
(_@odata.nextLink_ 応答ヘッダーに含まれる) か、_deltaToken_ (_@odata.deltaLink_ 応答ヘッダーに含まれる) のいずれかになります。前者はその回を続行する必要があることを示し、後者はその回のすべての変更の取得が完了したことを示します。

以下の応答は、_@odata.nextLink_ 応答ヘッダーに含まれる _skipToken_ を示しています。

注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/contactfolders/delta?$skiptoken={_skipToken_}",
  "value": [
    {
     "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "wellKnownName": "wellKnownName-value",
      "id": "id-value"
    }
  ]
}
```

### <a name="see-also"></a>関連項目

- [Microsoft Graph デルタ クエリ](/graph/delta-query-overview)
- [フォルダー内のメッセージへの増分の変更を取得する](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contactFolder: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
