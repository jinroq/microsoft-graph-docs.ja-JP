---
title: Bookingstaffmember の更新
description: 指定した bookingbusiness の bookingStaffMember のプロパティを更新します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: acfef7e88e6fe8d5bb8e46c5d3c3e3c85ff1aa33
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635891"
---
# <a name="update-bookingstaffmember"></a>Bookingstaffmember の更新

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定した[bookingbusiness](../resources/bookingbusiness.md)の[bookingStaffMember](../resources/bookingstaffmember.md)のプロパティを更新します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  予約します。すべての予約   |
|委任 (個人用 Microsoft アカウント) | サポートされていません。   |
|アプリケーション | サポートされていません。  |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-request-headers"></a>オプションの要求ヘッダー
| 名前       | 説明|
|:-----------|:-----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|availabilityIsAffectedByPersonalCalendar|Boolean|True は、スタッフメンバーが Office 365 ユーザーの場合、予約 API は、Office 365 のスタッフメンバーの個人用予定表と**workingHours**プロパティを使用して、可用性を判断します。 |
|colorIndex|Int32|スタッフメンバーを表す色を識別します。 この色は、予約アプリの [**スタッフの詳細**] ページのカラーパレットに対応しています。|
|displayName|String|スタッフメンバーの名前。顧客に表示されます。|
|emailAddress|String|スタッフメンバーの電子メールアドレス。 これは、ビジネスと同じ Office 365 テナント内、または別の電子メールドメインに配置できます。 この電子メールアドレスは、ビジネスのスケジューリングポリシーで**sendConfirmationsToOwner**プロパティが true に設定されている場合に使用されます。|
|role|string| 業務のスタッフメンバーの役割。 使用可能な値は、`guest`、`administrator`、`viewer`、`externalGuest` です。|
|useBusinessHours|Boolean|True は、スタッフメンバーの利用可能性がビジネスの**microsoft.rtc.rgs.management.writablesettings.businesshours**プロパティによって決定されることを意味します。 False は、可用性がスタッフメンバーの**workingHouse**プロパティの設定によって決定されることを意味します。|
|workingHours|[Bookingwork hours](../resources/bookingworkhours.md)コレクション|スタッフメンバーが予約に使用できる各曜日の時間の範囲。|

## <a name="response"></a>応答
成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。
## <a name="example"></a>例
##### <a name="request"></a>要求
次の例では、スタッフメンバーのスケジュールを変更して月曜日をオフにします。
<!-- {
  "blockType": "request",
  "name": "update_bookingstaffmember"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/8ee1c803-a1fa-406d-8259-7ab53233f148
Content-type: application/json

{
    "workingHours":[
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"monday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[

            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"tuesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"wednesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"thursday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"friday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        }
    ]
}
```
##### <a name="response"></a>応答
応答の例を次に示します。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/update_bookingstaffmember-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_bookingstaffmember-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingstaffmember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingstaffmember-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingstaffmember-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
