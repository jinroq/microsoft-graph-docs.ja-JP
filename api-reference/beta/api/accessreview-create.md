---
title: AccessReview を作成する
description: Azure AD access レビュー機能で、新しい accessReview オブジェクトを作成します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8a462398903a821bba1022cde07f45f99817356c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33586462"
---
# <a name="create-accessreview"></a>AccessReview を作成する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、新しい[accessreview](../resources/accessreview.md)オブジェクトを作成します。

この要求を行う前に、発信者は以前に[ビジネスフローテンプレートの一覧を取得](businessflowtemplate-list.md)して、の`businessFlowTemplateId`値を要求に含める必要があります。

この要求を行った後、呼び出し元は、プログラムにアクセスレビューをリンクするために[programControl を作成](programcontrol-create.md)する必要があります。  

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | AccessReview.ReadWrite.All |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | サポートされていません。 |

また、呼び出し元は、アクセスレビューを作成した後、プログラムの[制御](../resources/programcontrol.md)を作成できるようにするために、プログラムによる制御が必要になります。
さらに、サインインしているユーザーも、アクセスレビューを作成することを許可するディレクトリロールにある必要があります。  詳細については、「[アクセスレビュー](../resources/accessreviews-root.md)の役割とアクセス許可の要件」を参照してください。

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a>要求ヘッダー
| 名前         | 型        | 説明 |
|:-------------|:------------|:------------|
| Authorization | string | ベアラー \{トークン\}。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、 [Accessreview](../resources/accessreview.md)オブジェクトの JSON 表記を指定します。

次の表に、accessReview の作成時に必要なプロパティを示します。

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | アクセスレビュー名。  |
| `startDateTime`           |`DateTimeOffset`                                                | レビューが開始される予定の日時。  これは、将来の日付である必要があります。   |
| `endDateTime`             |`DateTimeOffset`                                                | レビューが終了する予定の日時。 これは、開始日よりも1日以上後でなければなりません。   |
| `description`             |`String`                                                        | レビュー担当者に表示する説明。 |
| `businessFlowTemplateId`  |`String`                                                        | [Businessflowtemplate](../resources/businessflowtemplate.md)から取得したビジネスフローテンプレートの識別子。  |
| `reviewerType`            |`String`                                                        | レビュー対象のオブジェクトのアクセス権に対するレビュー担当者の関係の種類`self`、 `delegated`いずれか`entityOwners`、または。 | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | アクセスレビューが作成されるオブジェクト (グループのメンバーシップ、アプリケーションに対するユーザーの割り当てなど)。 | 


指定した reviewerType に値`delegated`がある場合は、レビュー担当者にも`reviewers`プロパティが含まれている必要があります。これには、レビューアーの[useridentity](../resources/useridentity.md)のコレクションが含まれています。

アプリが、サインインしているユーザーなしでこの API を呼び出している場合は、発信者にも**createdBy**プロパティが含まれている必要があります。この値は、レビューの作成者として識別されるユーザーの[useridentity](../resources/useridentity.md)です。

また、呼び出し元には、定期的なレビューのシリーズを作成したり、既定のレビュー動作から変更したりするための設定を含めることができます。 特に、定期的なレビューを作成するには、呼び出し元`accessReviewRecurrenceSettings`に、アクセスレビュー設定内にを含める必要があります。


## <a name="response"></a>応答
成功した場合、このメソッド`201, Created`は応答コードと、応答本文で[accessreview](../resources/accessreview.md)オブジェクトを返します。

## <a name="example"></a>例

これは、1回限り (繰り返しではない) アクセスレビューを作成し、2人のユーザーをレビュー担当者として明示的に指定する例です。

##### <a name="request"></a>要求
要求本文で、 [Accessreview](../resources/accessreview.md)オブジェクトの JSON 表記を指定します。

<!-- {
  "blockType": "request",
  "name": "create_accessReview_from_accessReviews"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews
Content-type: application/json

{
    "displayName":"TestReview",
    "startDateTime":"2017-02-10T00:35:53.214Z",
    "endDateTime":"2017-03-12T00:35:53.214Z",
    "reviewedEntity": {
        "id": "99025615-a0b1-47ec-9117-35377b10998b",
    },
    "reviewerType" : "delegated",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "description":"Sample description",
    "reviewers":
    [
        {
            "id":"f260246a-09b1-4fd5-8d18-daed736071ec"
        },
        {
            "id":"5a4e184c-4ee5-4883-96e9-b371f8da88e3"
        }
    ],
    "settings":
    {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval":true,
        "autoReviewEnabled":false,
        "activityDurationInDays":30,
        "autoApplyReviewResultsEnabled":false,
        "accessRecommendationsEnabled":false,
        "recurrenceSettings":{
            "recurrenceType":"onetime",
            "recurrenceEndType":"endBy",
            "durationInDays":0,
            "recurrenceCount":0
        },
        "autoReviewSettings":{
            "notReviewedResult":"Deny"
        }
    }
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
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegated",
    "description": "Sample description"
}
```
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/create_accessReview_from_accessReviews-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_accessReview_from_accessReviews-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "Create accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-create.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-create.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
