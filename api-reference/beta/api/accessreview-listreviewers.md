---
title: AccessReview レビュー担当者のリスト
description: Azure AD access レビュー機能で、accessReview オブジェクトのレビュー担当者を取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9890df72f00d223f169b80ae2ba277560ccf5c72
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440044"
---
# <a name="list-accessreview-reviewers"></a>AccessReview レビュー担当者のリスト

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、 [accessreview](../resources/accessreview.md)オブジェクトのレビュー担当者を取得します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | AccessReview を参照してください。 |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | AccessReview.Read.All  |


 また、サインインしているユーザーは、アクセスレビューを読み取ることができるようにするためのディレクトリロールにある必要があります。

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a>要求ヘッダー
| 名前         | 型        | 説明 |
|:-------------|:------------|:------------|
| Authorization | string | ベアラー \{トークン\}。必須。 |

## <a name="request-body"></a>要求本文
要求本文を指定する必要はありません。

## <a name="response"></a>応答
成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[useridentity](../resources/useridentity.md)オブジェクトの配列を返します。

## <a name="example"></a>例
##### <a name="request"></a>要求


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-reviewers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-reviewers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-reviewers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
    "value":
    [
        {
            "id":"006111db-0810-4494-a6df-904d368bd81b"
        }
    ]
}
```

## <a name="see-also"></a>関連項目

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[AccessReview を取得する](accessreview-get.md) |  [accessReview](../resources/accessreview.md) |  アクセスレビューを取得します。 |
|[AccessReview レビュー担当者を追加する](accessreview-addreviewer.md) |     なし。   |   閲覧者を accessReview に追加します。 |
|[AccessReview レビュー担当者を削除する](accessreview-removereviewer.md) | なし。 |   AccessReview からレビュー担当者を削除します。 |


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
