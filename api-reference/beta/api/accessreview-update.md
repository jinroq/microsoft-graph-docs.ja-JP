---
title: AccessReview を更新します。
description: Azure AD アクセスのレビュー機能では、1 つまたは複数のプロパティを変更するのには既存の accessReview オブジェクトを更新します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1256ccdabea8eb5c0c0ffb3365e0c87276999236
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524367"
---
# <a name="update-accessreview"></a>AccessReview を更新します。

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、1 つまたは複数のプロパティを変更するのには既存の[accessReview](../resources/accessreview.md)オブジェクトを更新します。

レビュー担当者やレビューの決定を変更するのには、この API は想定されていません。  レビュー担当者を変更するには、 [addReviewer](accessreview-addreviewer.md)または[removeReviewer](accessreview-removereviewer.md) Api を使用します。  すでに開始された 1 回限りのレビュー、または定期的なレビューの既に起動インスタンスを停止するには、初期の段階では、[停止する](accessreview-stop.md)API を使用します。 ターゲット ・ グループ、またはアプリケーションのアクセス権の決定を適用するには、[適用](accessreview-apply.md)API を使用します。 


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
| Authorization | string | ベアラー トークン 必須です。 |

## <a name="request-body"></a>要求本文
要求の本文に、JSON 形式の[accessReview](../resources/accessreview.md)オブジェクトのパラメーターを指定します。

次の表は、accessReview を更新するときに指定できるプロパティを示しています。

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | アクセス確認の名前です。  |
| `startDateTime`           |`DateTimeOffset`                                                | 日付と時刻と、レビューを開始する予定です。  将来の日付でなければなりません。   |
| `endDateTime`             |`DateTimeOffset`                                                | レビューの終了がスケジュールされているときの日時。 これは、少なくとも 1 つの日を開始日より後でなければなりません。   |
| `description`             |`String`                                                        | 校閲者を表示する説明します。 |



## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`204, Accepted`応答コードおよび応答の本文内の[accessReview](../resources/accessreview.md)オブジェクトです。

## <a name="example"></a>例

これは、1 回限り (繰り返し発生しない) のアクセス確認の更新の例です。

##### <a name="request"></a>要求
要求の本文には、 [accessReview](../resources/accessreview.md)オブジェクトの新しいプロパティの JSON 表現を指定します。

<!-- {
  "blockType": "request",
  "name": "update_accessReview"
}-->
```http
PATCH https://graph.microsoft.com/beta/accessReviews('006111db-0810-4494-a6df-904d368bd81b')
Content-type: application/json

{
    "displayName":"TestReview new name"
}
```

##### <a name="response"></a>応答
>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
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
    "Error: /api-reference/beta/api/accessreview-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
