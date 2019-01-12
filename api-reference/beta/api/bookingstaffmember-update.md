---
title: Bookingstaffmember を更新します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 597647d86df8f34c7fb9a7eba93a5eccc1129f6c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952224"
---
# <a name="update-bookingstaffmember"></a>Bookingstaffmember を更新します。

 > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。
 
指定された[bookingbusiness](../resources/bookingbusiness.md)では、 [bookingStaffMember](../resources/bookingstaffmember.md)のプロパティを更新します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  Bookings.ReadWrite.All、Bookings.Manage.All   |
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

| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|availabilityIsAffectedByPersonalCalendar|Boolean|True は、スタッフ メンバーが、Office 365 ユーザーの場合は、予約 API は**workingHours**プロパティと同様に Office 365 で、スタッフ メンバーの個人用予定表の可用性を決定します。 |
|colorIndex|Int32|スタッフ メンバーを表す色を識別します。 予約アプリケーションでは、**スタッフの詳細**ページでカラー パレットに色が対応しています。|
|displayName|String|顧客に表示されるよう、スタッフ メンバーの名前です。|
|emailAddress|String|スタッフ メンバーの電子メール アドレスです。 ビジネスとして同じ Office 365 テナントにまたは別の電子メール ドメインを指定できます。 **SendConfirmationsToOwner**プロパティが設定されている場合、この電子メール アドレスが使用されるビジネスのスケジュー リング ポリシーの場合は true です。|
|role|string| ビジネスのスタッフの役割です。 可能な値は、`guest`、`administrator`、`viewer`、`externalGuest` です。|
|useBusinessHours|Boolean|True では、スタッフ メンバーの可用性は、ビジネスの**businessHours**プロパティによって決定されることを意味します。 False は、利用可能時間は、スタッフ メンバーの**workingHouse**プロパティの設定によって決定されますを意味します。|
|workingHours|[bookingWorkHours](../resources/bookingworkhours.md)コレクション|スタッフ メンバーは、予約に使用される 1 週間の各日の時間の範囲です。|

## <a name="response"></a>応答
成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。
## <a name="example"></a>例
##### <a name="request"></a>要求
次の使用例では、毎週月曜日にのスタッフ メンバーのスケジュールを変更します。
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update bookingstaffmember",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
