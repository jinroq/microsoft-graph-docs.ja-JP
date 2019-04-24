---
title: plannerRecentPlanReference リソースの種類
description: '**plannerRecentPlanReference**リソースの種類表す workbookconnection は、ユーザーが最近表示した plan プランへの参照を示します。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 55ccf34055d7d181dbbeecd5b6c30a3843f211d5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522154"
---
# <a name="plannerrecentplanreference-resource-type"></a>plannerRecentPlanReference リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**plannerRecentPlanReference**リソースの種類表す workbookconnection は、ユーザーが最近表示した[plan プラン](plannerplan.md)への参照を示します。 ユーザーの**plannerRecentPlanReferences**は、アプリによって明示的に管理されます。 最近のプランを実装するすべてのアプリは、ユーザーが前回プランを表示したときに記録し、それに応じて**plannerRecentPlanReference**エントリを更新する必要があります。
**plannerRecentPlanReference**エントリは、削除された**プラン**、ユーザーがアクセスできなくなったプラン、または別のタイトルで更新されたプランを参照できることに注意してください。
アプリでは、相違点がある場合にユーザーに通知し、エントリを最新の状態に保つことをお勧めします。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|lastAccessedDateTime|DateTimeOffset|プランが最後にユーザーによって表示された日時。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerrecentplanreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
