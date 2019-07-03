---
title: AccessReview を取得する
description: 'Azure AD access レビュー機能で、accessReview オブジェクトを取得します。  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2255717631b4bbe6bc9e41e259dfb1e4c1c9d774
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440079"
---
# <a name="get-accessreview"></a>AccessReview を取得する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、 [accessreview](../resources/accessreview.md)オブジェクトを取得します。  

アクセスレビューのレビュー担当者を取得するには、 [List accessreview レビューアー](accessreview-listreviewers.md) API を使用します。 アクセスレビューの決定を取得するには、「[リストアクセスレビュー決定](accessreview-listdecisions.md)api」、または「 [My accessreview review 決定](accessreview-listmydecisions.md)api の一覧」を使用します。

これが定期的なアクセスレビューである場合は、 `instances`リレーションシップを使用して、アクセスレビューの過去、現在、および今後のインスタンスの[accessreview](../resources/accessreview.md)コレクションを取得します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | AccessReview.Read.All  |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | AccessReview.Read.All  |

この API を呼び出すためには、サインインしているユーザーが、アクセスレビューを読み取ることを許可するディレクトリロールにあるか、アクセスレビューのレビュー担当者としてユーザーを割り当てることも必要です。  詳細については、「[アクセスレビュー](../resources/accessreviews-root.md)の役割とアクセス許可の要件」を参照してください。

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a>要求ヘッダー
| 名前         | 型        | 説明 |
|:-------------|:------------|:------------|
| Authorization | string | ベアラー \{トークン\}。必須。 |

## <a name="request-body"></a>要求本文
要求本文を指定する必要はありません。

## <a name="response"></a>応答
成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[accessreview](../resources/accessreview.md)オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>応答
>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
    "displayName": "review",
    "startDateTime": "2017-11-14T01:14:54.89Z",
    "endDateTime": "2017-12-14T01:14:54.89Z",
    "status": "InProgress",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "self",
    "description": "",
    "reviewedEntity":{"id":"3b4f7e74-eb82-4120-9ff5-ba429c1ea6df","displayName":"Salesforce"},
    "settings": {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval": true,
        "autoReviewEnabled": false,
        "activityDurationInDays": 30,
        "autoApplyReviewResultsEnabled": false,
        "accessRecommendationsEnabled": false,
        "recurrenceSettings": {
            "recurrenceType": "onetime",
            "recurrenceEndType": "endBy",
            "durationInDays": 0,
            "recurrenceCount": 0
        },
        "autoReviewSettings": {
            "notReviewedResult": "Deny"
        }
    }
}
```

## <a name="see-also"></a>関連項目

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[AccessReview を作成する](accessreview-create.md) |    [accessReview](../resources/accessreview.md) |  新しい accessReview を作成します。 |
|[ProgramControls のリスト](programcontrol-list.md) | [Programcontrol](../resources/programcontrol.md)コレクション | テナント内の programControls を一覧表示します。 |
|[AccessReview レビュー担当者のリスト](accessreview-listreviewers.md) |     [Useridentity](../resources/useridentity.md)コレクション|    AccessReview のレビュー担当者を取得します。 |
|[AccessReview に関する決定事項を一覧表示する](accessreview-listdecisions.md) |     [accessReviewDecision](../resources/accessreviewdecision.md)コレクション|    AccessReview の決定事項を取得します。|
|[自分の accessReview の決定事項を一覧表示する](accessreview-listmydecisions.md) |        [accessReviewDecision](../resources/accessreviewdecision.md)コレクション|    レビュー担当者として、accessReview の決定事項を取得します。|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
