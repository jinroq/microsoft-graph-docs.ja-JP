---
title: scheduleInformation リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
ms.openlocfilehash: e84505ee2f30a5b7b52e9d5b589b8bb24d9a4c95
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521909"
---
# <a name="scheduleinformation-resource-type"></a>scheduleInformation リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
指定された期間内のユーザー、配布リスト、またはリソースの可用性を表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|availabilityView |String |マージされたビュー内のすべての項目の数を表す`scheduleItems`。 ビューは、時間帯で構成されています。 各時間帯の可用性で示されます。:`0`無料 = `1`= 仮の予定、 `2`= ビジー状態か、`3`外出中 = `4`= の別の場所で作業します。|
|エラー |[freeBusyError](freebusyerror.md) |エラー情報が、ユーザー、配布リスト、またはリソースの可用性を取得しようとしていますから。 |
|scheduleId |String |ユーザー、配布リスト、または**scheduleInformation**のインスタンスを識別する、リソースの SMTP アドレスです。 |
|scheduleItems |[scheduleItem](scheduleitem.md)コレクション |ユーザーまたはリソースの可用性を説明する項目が含まれています。 |
|workingHours |[workingHours](workinghours.md) |ユーザーが働く曜日と、特定のタイムゾーンの時間。 これらは、ユーザーの[mailboxSettings](mailboxsettings.md)の一部として設定されています。|


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleInformation"
}-->

```json
{
  "availabilityView": "String",
  "error": {"@odata.type": "microsoft.graph.freeBusyError"},
  "scheduleId": "String",
  "scheduleItems": [{"@odata.type": "microsoft.graph.scheduleItem"}],
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scheduleinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
