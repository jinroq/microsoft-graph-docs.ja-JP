---
title: AccessReview レビュー担当者を削除する
description: 'Azure AD access レビュー機能で、既存の accessReview オブジェクトを更新して、ユーザーを校閲者として削除します。  この操作は、まだ完了していないアクセスレビューに対してのみ許可されており、レビュー担当者が明示的に指定されているアクセスレビューに対してのみ使用できます。 この操作は、ユーザーが自分のアクセスを確認するアクセスレビューでは許可されず、グループの所有者がレビュー担当者として割り当てられているアクセスレビューのためのものではありません。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c0b5407b07f309a1c6e7e5e8e6bd0942ad8aca23
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655538"
---
# <a name="remove-accessreview-reviewer"></a>AccessReview レビュー担当者を削除する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、既存の[accessreview](../resources/accessreview.md)オブジェクトを更新して、ユーザーを校閲者として削除します。  この操作は、まだ完了していないアクセスレビューに対してのみ許可されており、レビュー担当者が明示的に指定されているアクセスレビューに対してのみ使用できます。 この操作は、ユーザーが自分のアクセスを確認するアクセスレビューでは許可されず、グループの所有者がレビュー担当者として割り当てられているアクセスレビューのためのものではありません。 


## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | AccessReview.ReadWrite.All |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('{reviewId}')/reviewers('{userId'})
```
## <a name="request-headers"></a>要求ヘッダー
| 名前         | 型        | 説明 |
|:-------------|:------------|:------------|
| Authorization | string | ベアラー \{トークン\}。必須。 |

## <a name="request-body"></a>要求本文
要求本文を指定する必要はありません。


## <a name="response"></a>応答
成功した場合、このメソッドは200シリーズの応答コードを返します。

## <a name="example"></a>例

これは、不要なレビューを削除するために、1回限り (定期的でない) アクセスレビューを更新する例です。


##### <a name="request"></a>要求
要求 URL で、accessReview オブジェクトの id と、ユーザーオブジェクトの id を指定します。

<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers/006111db-0810-4494-a6df-904d368bd81b

```

##### <a name="response"></a>応答
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a>SDK サンプル コード
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/remove_accessReview_reviewer-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/remove_accessReview_reviewer-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "Remove accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-removereviewer.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-removereviewer.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
