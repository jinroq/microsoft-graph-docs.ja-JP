---
title: synchronizationJobRestartCriteria リソースの種類
description: 'スコープを定義します[synchronizationJob: 再起動](../api/synchronization_synchronizationjob_restart.md)アクション。'
localization_priority: Normal
ms.openlocfilehash: 1e6ac952808f80d191fc93e9a804411ec4459d4c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642521"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a>synchronizationJobRestartCriteria リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

スコープを定義します[synchronizationJob: 再起動](../api/synchronization_synchronizationjob_restart.md)アクション。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|resetScope|String| 次の値のコンマ区切りの組み合わせ: `Full`、 `QuarantineState`、 `Watermark`、 `Escrows`、 `ConnectorDataStore`。 使用`Full`のすべてのオプションにする場合。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}-->

```json
{
  "resetScope": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationjobrestartcriteria.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
