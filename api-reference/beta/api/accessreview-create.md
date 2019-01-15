---
title: AccessReview を作成します。
description: Azure AD のレビュー機能にアクセス、新しい accessReview オブジェクトを作成します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: de8574566a8ca1eedb1f0f55230fb91053370ccc
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016724"
---
# <a name="create-accessreview"></a>AccessReview を作成します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、新しい[accessReview](../resources/accessreview.md)オブジェクトを作成します。

この要求を行う前に呼び出し元には以前[業務フローのテンプレートの一覧を取得](businessflowtemplate-list.md)するにはの値を設定する`businessFlowTemplateId`要求に含める。

呼び出し元では、この要求を行った後[、デバッギングを作成](programcontrol-create.md)、アクセス確認をプログラムにリンクする必要があります。  

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | AccessReview.ReadWrite.All、デバッギングを作成する後続の呼び出しで完全なシナリオを ProgramControl.ReadWrite.All する必要があり、 |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a>要求ヘッダー
| 名前         | 型        | 説明 |
|:-------------|:------------|:------------|
| Authorization | string | ベアラー\{トークン\}。 必須。 |

## <a name="request-body"></a>要求本文
要求の本文には、 [accessReview](../resources/accessreview.md)オブジェクトの JSON 表現を指定します。

次の表は、accessReview を作成するときに必要なプロパティを示します。

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | アクセス確認の名前です。  |
| `startDateTime`           |`DateTimeOffset`                                                | 日付と時刻と、レビューを開始する予定です。  将来の日付でなければなりません。   |
| `endDateTime`             |`DateTimeOffset`                                                | レビューの終了がスケジュールされているときの日時。 これは、少なくとも 1 つの日を開始日より後でなければなりません。   |
| `description`             |`String`                                                        | 校閲者を表示する説明します。 |
| `businessFlowTemplateId`  |`String`                                                        | ビジネス フロー テンプレート識別子の[businessFlowTemplate](../resources/businessflowtemplate.md)から取得します。  |
| `reviewerType`            |`String`                                                        | リレーションシップの種類のいずれかの確認済みのオブジェクトのアクセス許可の校閲者の`self`、 `delegated`、または`entityOwners`。 | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | アクセス確認を作成するため、グループのメンバーシップなどのユーザーがアプリケーションの割り当てオブジェクトです。 | 


指定された reviewerType に値が設定されている場合`delegated`、呼び出し元は含める必要がありますし、`reviewers`プロパティは、一連の校閲者に[割り当てられていません](../resources/useridentity.md)。

さらに、呼び出し元は、一連の定期的なレビューを作成するか、既定の確認動作を変更する設定を含めることができます。 具体的には、定期的なレビューを作成するには、呼び出し元する必要があります、 `accessReviewRecurrenceSettings` 、access 内で設定を確認します


## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`201, Created`応答コードおよび応答の本文内の[accessReview](../resources/accessreview.md)オブジェクトです。

## <a name="example"></a>例

これは、校閲者として、2 人のユーザーを明示的に指定する 1 回限り (定期ではない) アクセス確認を作成する例です。

##### <a name="request"></a>要求
要求の本文には、 [accessReview](../resources/accessreview.md)オブジェクトの JSON 表現を指定します。

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

<!-- {
  "type": "#page.annotation",
  "description": "Create accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
