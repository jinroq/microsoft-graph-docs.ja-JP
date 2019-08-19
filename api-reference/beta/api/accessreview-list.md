---
title: AccessReviews をリストする
description: BusinessFlowTemplate の accessReview オブジェクトを取得します。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 46c9abdbc0a1d5dca4c4e61d423b23ed31691384
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/19/2019
ms.locfileid: "36462658"
---
# <a name="list-accessreviews"></a>AccessReviews をリストする

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定の[Businessflowtemplate](../resources/businessflowtemplate.md)の[accessreview](../resources/accessreview.md)オブジェクトを取得します。 そのビジネスフローテンプレートを使用して作成された1回限りのアクセスレビューおよび定期的なアクセスレビューごとに、0個以上の**Accessreview**オブジェクトのリストが返されます。

>[!NOTE]
> フィルターに一致するいずれかのアクセスレビューが定期的なアクセスレビューである場合は、1つの**accessreview**オブジェクトが返され、定期的な各シリーズが全体として表現されます。 たとえば、グループ A のゲストメンバーに対する定期的なアクセスのレビュー、グループ B のゲストメンバーに対する定期的なアクセスレビュー、グループ C のゲストメンバーの1回限りのアクセスレビュー、および呼び出し元がビジネスフローを使用したアクセスレビューを照会する場合は、グループのゲストメンバーのレビューのテンプレート。3つのオブジェクトが返されます。 定期的なアクセスレビューのインスタンス、または特定の月または四半期に対してスケジュールされたアクセスレビューインスタンスを取得するには、その後、呼び出し元が定期的な**Accessreview**オブジェクトの**インスタンス**リレーションシップを移動できます。 **インスタンス**リレーションシップは、定期的なアクセスレビューの現在のインスタンスまたは過去のインスタンスの**accessreview**オブジェクトにリンクします。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | Accessreview を参照してください。この後、accessreview を参照してください。  |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | AccessReview を参照してください。 |

 また、サインインしているユーザーは、アクセスレビューを読み取ることができるようにするためのディレクトリロールにある必要があります。

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews?$filter=businessFlowTemplateId eq {businessFlowTemplate-id}
```
## <a name="request-headers"></a>要求ヘッダー
| 名前         | 型        | 説明 |
|:-------------|:------------|:------------|
| Authorization | string | ベアラー \{トークン\}。必須。 |

## <a name="request-body"></a>要求本文
要求本文を指定しません。

## <a name="response"></a>応答
成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[accessreview](../resources/accessreview.md)オブジェクトの配列を返します。

## <a name="examples"></a>例
##### <a name="request"></a>要求
次の例は、ビジネスフローテンプレート ' 6E4F3D20-C5C3-407F-9695-8460952BCC68 ' に対して1回限りの定期的なアクセスレビューをすべて取得する要求を示しています。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviews"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews?$filter=businessFlowTemplateId+eq+'6E4F3D20-C5C3-407F-9695-8460952BCC68'
```


---


##### <a name="response"></a>応答
>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
       {
         "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
         "displayName": "review",
         "startDateTime": "2017-11-14T01:14:54.89Z",
         "endDateTime": "2017-12-14T01:14:54.89Z",
         "status": "InProgress",
         "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
         "reviewerType": "self",
         "description": "",
         "reviewedEntity":{"id":"3b4f7e74-eb82-4120-9ff5-ba429c1ea6df","displayName":"Salesforce"}
       }
    ]
}
```

## <a name="see-also"></a>関連項目

- [AccessReview を取得する](accessreview-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReviews",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
