---
title: synchronizationQuarantine リソースの種類
description: SynchronizationJob の検査の状態に関する情報を提供します。
localization_priority: Normal
ms.openlocfilehash: 6d5d5c3cbe96eda6b39833287e8efb6e0771b19a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518815"
---
# <a name="synchronizationquarantine-resource-type"></a>synchronizationQuarantine リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

の[synchronizationJob](synchronization-synchronizationjob.md)の検査の状態に関する情報を提供します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|currentBegan|DateTimeOffset|日付と時刻の検査が最後に評価され、課されます。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。|
|nextAttempt|DateTimeOffset|日付と時刻、次が再検査を評価しようとした場合に行われます。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。|
|理由|String|検疫が適用された理由を示すコードです。 可能な値は、`EncounteredBaseEscrowThreshold`、`EncounteredTotalEscrowThreshold`、`EncounteredEscrowProportionThreshold`、`EncounteredQuarantineException`、`Unknown` です。|
|seriesBegan|DateTimeOffset|日付と時刻の検査が最初にこのシリーズ (シリーズを開始すると、検疫が最初に適用されると、隔離が解除されると、すぐにリセットされます) に課されます。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。|
|seriesCount|Int64|このシリーズは、検査の回数が再評価し、左 (シリーズ開始と検査は、最初に適用されると、隔離が解除されると、すぐにリセットされます) では有効にします。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationQuarantine"
}-->

```json
{
  "currentBegan": "String (timestamp)",
  "nextAttempt": "String (timestamp)",
  "reason": "String",
  "seriesBegan": "String (timestamp)",
  "seriesCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationQuarantine resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-quarantine.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
