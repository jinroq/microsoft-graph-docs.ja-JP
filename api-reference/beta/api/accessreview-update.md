---
title: AccessReview を更新します。
description: Azure AD アクセスのレビュー機能では、1 つまたは複数のプロパティを変更するのには既存の accessReview オブジェクトを更新します。
localization_priority: Normal
ms.openlocfilehash: 65420b3682eb9d9f72d95beea624eb84429628ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833748"
---
# <a name="update-accessreview"></a>AccessReview を更新します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、1 つまたは複数のプロパティを変更するのには既存の[accessReview](../resources/accessreview.md)オブジェクトを更新します。

レビュー担当者やレビューの決定を変更するのには、この API は想定されていません。  レビュー担当者を変更するには、 [addReviewer](accessreview-addreviewer.md)または[removeReviewer](accessreview-removereviewer.md) Api を使用します。  すでに開始された 1 回限りのレビュー、または定期的なレビューの既に起動インスタンスを停止、[停止](accessreview-stop.md)API を使用して、初期の段階では、ターゲット ・ グループまたはアプリケーション アクセス権の決定に適用する、[適用](accessreview-apply.md)API を使用して、します。 


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
| 名前         | 種類        | 説明 |
|:-------------|:------------|:------------|
| Authorization | string | ベアラー\{トークン\}。 必須。 |

## <a name="request-body"></a>要求本文
要求の本体の[accessReview](../resources/accessreview.md)オブジェクトのパラメーターの JSON の形式を指定します。

次の表は、accessReview を更新するときに指定できるプロパティを示しています。

| プロパティ     | 種類        | 説明 |
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
    "reviewerType": "delegate",
    "description": "Sample description"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
