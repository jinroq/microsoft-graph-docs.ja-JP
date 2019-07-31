---
title: bookingSchedulingPolicy リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 77b1cf812edd334197c268c92bb982954fb11b12
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974123"
---
# <a name="bookingschedulingpolicy-resource-type"></a>bookingSchedulingPolicy リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Microsoft の予約予定表で予定を作成する方法を決定する一連のポリシーを表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowStaffSelection|Boolean|True の場合、ユーザーは予約の特定のユーザーを選択することができます。|
|maximumAdvance|期間|予約を事前に作成できる最大日数。 [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式に従います。|
|minimumLeadTime|期間|予約と取り消しを行う必要のある最小時間。 [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式に従います。|
|sendConfirmationsToOwner|Boolean| True は、予約が作成または変更されたときに電子メールでビジネスに通知します。 会社の**Bookingbusiness**エンティティの**email**プロパティで指定された電子メールアドレスを使用します。 |
|timeSlotInterval|期間|各時間帯の期間は、 [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で示されます。|

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingSchedulingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
