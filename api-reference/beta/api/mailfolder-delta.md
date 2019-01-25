---
title: 'mailFolder: delta'
description: ユーザーのメールボックスで追加または削除された一連のメール フォルダーを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b4aac9c0370084cd0c5450e304737a11c93dd8f7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522603"
---
# <a name="mailfolder-delta"></a>mailFolder: delta

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーのメールボックスで追加または削除された一連のメール フォルダーを取得します。

メールボックス内のメール フォルダーに対する**デルタ**関数の呼び出しと GET 要求とは似ていますが、[状態トークン](/graph/delta-query-overview)をこれらの呼び出しに適切に適用することにより、メール フォルダーの増分の変更をクエリできる点が異なります。これにより、ユーザーのメール フォルダーのローカル ストアの保守と同期を行う際に、そのメールボックスのメール フォルダーすべてを毎回サーバーからフェッチする必要がなくなります。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Mail.Read、Mail.ReadWrite    |
|委任 (個人用 Microsoft アカウント) | Mail.Read、Mail.ReadWrite    |
|アプリケーション | Mail.Read、Mail.ReadWrite |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/delta
GET /users/<id>/mailFolders/delta
```

## <a name="query-parameters"></a>クエリ パラメーター

メール フォルダーの変更を追跡すると、1 つ以上の **デルタ**関数呼び出しのラウンドが発生します。任意のクエリ パラメーター (`$deltatoken` と `$skiptoken` 以外) を使用する場合は、最初の**デルタ**要求でこれを指定する必要があります。Microsoft Graph は、応答で提供される `nextLink` や `deltaLink` の URL のトークン部分に指定したパラメーターを自動的にエンコードします。必要なクエリ パラメーターを前もって指定しておくだけで済みます。それ以降の要求では、前の応答で `nextLink` や `deltaLink` の URL に必要なパラメーターが既にエンコードされ、含まれているため、この URL をコピーして適用するだけです。

| クエリ パラメーター      | 種類   |説明|
|:---------------|:--------|:----------|
| $deltatoken | string | 同じメール フォルダー コレクションの前の**デルタ**関数呼び出しの `deltaLink` URL で[状態トークン](/graph/delta-query-overview)が返され、その変更追跡のラウンドが完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。|
| $skiptoken | string | 前の**デルタ**関数呼び出しの `nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じメール フォルダー コレクションに追跡すべき変更が他にもあることを示します。 |

### <a name="odata-query-parameters"></a>OData クエリ パラメーター

任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。 

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明 |
|:---------------|:----------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |
| Content-Type  | string  | application/json. Required. |
| Prefer | string  | odata.maxpagesize={x}.省略可能。 |

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mailFolder](../resources/mailfolder.md) コレクション オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求
次の例に、**デルタ**関数呼び出しを 1 つ作成し、応答本文に含まれるメール フォルダーの最大数を 2 に制限する方法を示します。

メールボックスのメール フォルダー内の変更を追跡するには、1 つ以上の**デルタ**関数呼び出しを作成し、適切な状態トークンを使用して、前回のデルタ クエリ以降になされた一連の増分の変更を取得します。 

メール フォルダー内のメッセージ変更を追跡するために状態トークンを使用する方法を示す同様の例については、次をご覧ください。「[フォルダー内のメッセージへの増分の変更を取得する](/graph/delta-query-messages)」。メール フォルダーの追跡とフォルダー内のメッセージの追跡の主な違いは、デルタ クエリ要求 URL と、**message** コレクションではなく **mailFolder** を返すクエリ応答にあります。

<!-- {
  "blockType": "request",
  "name": "mailfolder_delta"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/delta

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a>応答

要求が成功すると、応答には状態トークンが含まれます。これは、_skipToken_  
(_@odata.nextLink_ 応答ヘッダーに含まれる) か、_deltaToken_ (_@odata.deltaLink_ 応答ヘッダーに含まれる) のいずれかになります。前者はその回を続行する必要があることを示し、後者はその回のすべての変更の取得が完了したことを示します。

以下の応答は、_@odata.nextLink_ 応答ヘッダーに含まれる _skipToken_ を示しています。

注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/mailfolders/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "wellKnownName": "wellKnownName-value"
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
  "description": "mailFolder: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
