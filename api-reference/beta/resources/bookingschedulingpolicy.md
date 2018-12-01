---
title: bookingSchedulingPolicy リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: 7a16e9a2ec4e64978dd3c20f7510cfd42d76e826
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069900"
---
# <a name="bookingschedulingpolicy-resource-type"></a>bookingSchedulingPolicy リソースの種類

 > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。
 
Microsoft 予約カレンダーで予定を作成する方法を決定するポリシーのセットを表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowStaffSelection|ブール値|顧客が予約の特定の人を選択できるようにする場合は true です。|
|maximumAdvance|Duration|日の事前に、予約が可能な最大数です。 [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式に依存します。|
|minimumLeadTime|Duration|最小限の時間の前にある予約とキャンセル行う必要があります。 [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式に依存します。|
|sendConfirmationsToOwner|ブール値| 予約を作成または変更されたときに電子メール経由でビジネスを通知する場合は true です。 ビジネスの**bookingBusiness**エンティティの**email**プロパティで指定された電子メール アドレスを使用します。 |
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