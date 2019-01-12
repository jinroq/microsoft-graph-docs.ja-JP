---
title: bookingSchedulingPolicy リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 039d76b00787c9bf2e4f0bee4eb927a7628a9e76
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914639"
---
# <a name="bookingschedulingpolicy-resource-type"></a>bookingSchedulingPolicy リソースの種類

 > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。
 
Microsoft 予約カレンダーで予定を作成する方法を決定するポリシーのセットを表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowStaffSelection|Boolean|顧客が予約の特定の人を選択できるようにする場合は true です。|
|maximumAdvance|Duration|日の事前に、予約が可能な最大数です。 [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式に依存します。|
|minimumLeadTime|Duration|最小限の時間の前にある予約とキャンセル行う必要があります。 [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式に依存します。|
|sendConfirmationsToOwner|Boolean| 予約を作成または変更されたときに電子メール経由でビジネスを通知する場合は true です。 ビジネスの**bookingBusiness**エンティティの**email**プロパティで指定された電子メール アドレスを使用します。 |
|timeSlotInterval|Duration|[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で表される、各時間帯の期間です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingSchedulingPolicy"
}-->

```json
{
  "allowStaffSelection": true,
  "maximumAdvance": "String (timestamp)",
  "minimumLeadTime": "String (timestamp)",
  "sendConfirmationsToOwner": true,
  "timeSlotInterval": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingSchedulingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
