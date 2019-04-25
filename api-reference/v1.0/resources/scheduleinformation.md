---
title: scheduleinformation リソースの種類
description: 指定した期間のユーザー、配布リスト、またはリソースの空き時間情報を表します。
localization_priority: Normal
ms.openlocfilehash: a19689eeafe9723cdadeb6147700933ab171637c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579269"
---
# <a name="scheduleinformation-resource-type"></a>scheduleinformation リソースの種類

指定した期間のユーザー、配布リスト、またはリソース (会議室または備品) の空き時間情報を表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|availabilityView |String |のすべてのアイテムの利用可能時間のマージさ`scheduleItems`れたビューを表します。 ビューは、時間帯で構成されます。 各時間帯の可用性は、次の`0`ように表示`1`されます`2`。 = free `3`、= 仮設、= `4`busy、out 不在、または他の場所で動作します。|
|error |[freeBusyError](freebusyerror.md) |ユーザー、配布リスト、またはリソースの空き時間情報を取得しようとしたエラー情報。 |
|scheduleId |String |**scheduleinformation**のインスタンスを識別する、ユーザー、配布リスト、またはリソースの SMTP アドレス。 |
|scheduleitems |[scheduleitem](scheduleitem.md)コレクション |ユーザーまたはリソースの空き時間情報を示す項目を含みます。 |
|workingHours |[workingHours](workinghours.md) |ユーザーが働く曜日と、特定のタイムゾーンの時間。 これらは、ユーザーの[mailboxSettings](mailboxsettings.md)の一部として設定されます。|


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
  "tocPath": ""
}
-->
