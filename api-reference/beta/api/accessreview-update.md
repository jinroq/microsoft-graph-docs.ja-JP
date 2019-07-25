---
title: AccessReview を更新する
description: Azure AD access レビュー機能で、既存の accessReview オブジェクトを更新して、そのプロパティの1つ以上を変更します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7e290d7343fb7c5c34ce4952a97796dc94d080ae
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855908"
---
# <a name="update-accessreview"></a>AccessReview を更新する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、既存の[accessreview](../resources/accessreview.md)オブジェクトを更新して、そのプロパティの1つ以上を変更します。

この API は、レビュー担当者またはレビューの決定を変更するためのものではありません。  レビュー担当者を変更するには、 [Addreviewer](accessreview-addreviewer.md)または[removereviewer](accessreview-removereviewer.md) api を使用します。  既に開始した1回限りのレビュー、または定期的なレビューの事前に開始されているインスタンスを停止するには、 [stop](accessreview-stop.md) API を使用します。 目的のグループまたはアプリのアクセス権に決定を適用するには、[API の[適用](accessreview-apply.md)] を使用します。 


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
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a>要求ヘッダー
| 名前         | 型        | 説明 |
|:-------------|:------------|:------------|
| Authorization | string | ベアラー \{トークン\}。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、 [Accessreview](../resources/accessreview.md)オブジェクトのパラメーターの JSON 表記を指定します。

次の表に、accessReview の更新時に提供できるプロパティを示します。

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | アクセスレビュー名。  |
| `startDateTime`           |`DateTimeOffset`                                                | レビューが開始される予定の日時。  これは、将来の日付である必要があります。   |
| `endDateTime`             |`DateTimeOffset`                                                | レビューが終了する予定の日時。 これは、開始日よりも1日以上後でなければなりません。   |
| `description`             |`String`                                                        | レビュー担当者に表示する説明。 |



## <a name="response"></a>応答
成功した場合、このメソッド`204, Accepted`は応答コードと、応答本文で[accessreview](../resources/accessreview.md)オブジェクトを返します。

## <a name="example"></a>例

これは、1回限り (定期的でない) アクセスレビューを更新する例です。

##### <a name="request"></a>要求
要求本文で、 [Accessreview](../resources/accessreview.md)オブジェクトの新しいプロパティの JSON 表記を指定します。


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReview"
}-->
```http
PATCH https://graph.microsoft.com/beta/accessReviews/006111db-0810-4494-a6df-904d368bd81b
Content-type: application/json

{
    "displayName":"TestReview new name"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>応答
>**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
} -->
```http
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview new name",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegated",
    "description": "Sample description"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
