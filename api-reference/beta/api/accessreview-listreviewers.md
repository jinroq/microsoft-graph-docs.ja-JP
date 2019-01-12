---
title: AccessReview の校閲者の一覧
description: Azure AD にアクセスが機能を確認、校閲者の accessReview オブジェクトを取得します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8dca759f71f13af18c291f1af9843da6729ef701
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946813"
---
# <a name="list-accessreview-reviewers"></a>AccessReview の校閲者の一覧

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Azure AD[アクセスの確認](../resources/accessreviews-root.md)機能では、校閲者の[accessReview](../resources/accessreview.md)オブジェクトを取得します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | `AccessReview.Read.All`, `AccessReview.ReadWrite.All`.  サインインしているユーザーは、ディレクトリの役割をアクセスのレビューを読むことを許可する必要があります。 |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a>要求ヘッダー
| 名前         | 型        | 説明 |
|:-------------|:------------|:------------|
| Authorization | string | ベアラー\{トークン\}。 必須。 |

## <a name="request-body"></a>要求本文
要求の本体を提供する必要がありません。

## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`200, OK`応答コードおよび応答の本文に[割り当てられていません](../resources/useridentity.md)オブジェクトの配列。

## <a name="example"></a>例
##### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
```

##### <a name="response"></a>応答
>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userIdentity",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
       "id":"006111db-0810-4494-a6df-904d368bd81b"
    }
    ]
}
```

## <a name="see-also"></a>関連項目

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[AccessReview を取得します。](accessreview-get.md) |  [accessReview](../resources/accessreview.md) |  アクセス確認を取得します。 |
|[AccessReview の校閲者を追加します。](accessreview-addreviewer.md) |     なし。   |   AccessReview には、レビュー担当者を追加します。 |
|[AccessReview のレビュー担当者を削除します。](accessreview-removereviewer.md) | なし。 |   AccessReview からレビュー担当者を削除します。 |


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
