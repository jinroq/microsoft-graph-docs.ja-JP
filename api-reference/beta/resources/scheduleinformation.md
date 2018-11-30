---
title: scheduleInformation リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: 0b7bbd861a044b28cd22603fd0ccc27d20f46fba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069803"
---
# <a name="scheduleinformation-resource-type"></a>scheduleInformation リソースの種類

 > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。
 
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
<!-- {
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->