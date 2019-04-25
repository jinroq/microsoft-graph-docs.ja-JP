---
title: bookingwork hours リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 9a51fb9d4f97dde2e3b50d9a19481eeab31483d1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535492"
---
# <a name="bookingworkhours-resource-type"></a>bookingwork hours リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
1週間の稼働時間のセットを表します。これは、 [bookingbusiness](bookingbusiness.md)または[bookingStaffMember](bookingstaffmember.md)に対して使用されます。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|日勤|String| このインスタンスで表される曜日。 可能な値は、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。|
|timeSlots|[bookingwork timesロット](bookingworktimeslot.md)コレクション|1日の開始/終了時刻のリスト。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingWorkHours"
}-->

```json
{
  "day": "String",
  "timeSlots": [{"@odata.type": "microsoft.graph.bookingWorkTimeSlot"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingWorkHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingworkhours.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
