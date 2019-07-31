---
title: plannerRecentPlanReference リソースの種類
description: '**PlannerRecentPlanReference**リソースの種類表す workbookconnection は、ユーザーが最近表示した plan プランへの参照を示します。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8439502aa1214e1ef2bbedd9864ef4724abf8021
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965867"
---
# <a name="plannerrecentplanreference-resource-type"></a>plannerRecentPlanReference リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**PlannerRecentPlanReference**リソースの種類表す workbookconnection は、ユーザーが最近表示した[plan プラン](plannerplan.md)への参照を示します。 ユーザーの**plannerRecentPlanReferences**は、アプリによって明示的に管理されます。 最近のプランを実装するすべてのアプリは、ユーザーが前回プランを表示したときに記録し、それに応じて**plannerRecentPlanReference**エントリを更新する必要があります。
**PlannerRecentPlanReference**エントリは、削除された**プラン**、ユーザーがアクセスできなくなったプラン、または別のタイトルで更新されたプランを参照できることに注意してください。
アプリでは、相違点がある場合にユーザーに通知し、エントリを最新の状態に保つことをお勧めします。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|lastAccessedDateTime|DateTimeOffset|プランが最後にユーザーによって表示された日時。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|プランのタイトル|String|ユーザーが表示したときのプランのタイトル。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerRecentPlanReference"
}-->

```json
{
  "lastAccessedDateTime": "String (timestamp)",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerRecentPlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
