---
title: リストの accessReview の決定
description: Azure AD のレビュー機能にアクセス、accessReview オブジェクトの決定を取得します。
ms.openlocfilehash: d8cf89706f053dfee6e98cdf23d2539874ac6997
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067685"
---
# <a name="list-accessreview-decisions"></a>リストの accessReview の決定

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Azure AD[アクセスの確認](../resources/accessreviews-root.md)機能では、 [accessReview](../resources/accessreview.md)オブジェクトの決定を取得します。

定期的なアクセス確認がないことに注意を`decisions`の関係。  代わりに、呼び出し元が移動する必要があります、`instance`を検索するには、顧客間関係、`accessReview`アクセス レビューの現在または過去のインスタンスのオブジェクトです。

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
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a>要求ヘッダー
| 名前         | 型        | 説明 |
|:-------------|:------------|:------------|
| Authorization | string | ベアラー\{トークン\}。 必須。 |

## <a name="request-body"></a>要求本文
要求の本体を提供する必要がありません。

## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`200, OK`応答コードおよび応答の本文に[accessReviewDecision](../resources/accessreviewdecision.md)オブジェクトの配列。

## <a name="example"></a>例
##### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/decisions
```

##### <a name="response"></a>応答
>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewDecision",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
            "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "accessReviewId": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "reviewResult": "Approve",
            "userPrincipalName": "alice@litware.com",
            "userId": "Alice Smith"
    }
    ]
}
```

## <a name="see-also"></a>関連項目

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[AccessReview を取得します。](accessreview-get.md) |  [accessReview](../resources/accessreview.md) |  アクセス確認を取得します。 |
|[マイ accessReview の決定事項を表示します。](accessreview-listmydecisions.md) |        [accessReviewDecision](../resources/accessreviewdecision.md)コレクション|    参照者、accessReview の自分の意思決定を取得します。|
|[AccessReview アラームを送信します。](accessreview-sendreminder.md) |       なし。   |   AccessReview のレビュー担当者に通知を送信します。 |
|[AccessReview を停止します。](accessreview-stop.md) |        なし。   |   AccessReview を停止します。 |
|[リセット accessReview 決定](accessreview-reset.md) |        なし。   |   進行中の accessReview の決定をリセットします。|
|[AccessReview の決定を適用します。](accessreview-apply.md) |        なし。   |   完了した accessReview からの決定を適用します。|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
