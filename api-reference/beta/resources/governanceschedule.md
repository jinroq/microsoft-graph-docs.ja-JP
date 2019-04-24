---
title: governanceSchedule リソースの種類
description: 'governanceRoleAssignmentRequest のスケジュールを表します。 役割の割り当て要求の場合、スケジュールは、役割の割り当て操作を実行するタイミング、役割の割り当てを停止するタイミング、および役割の割り当て操作を実行する頻度を制御します。 '
localization_priority: Normal
ms.openlocfilehash: d7ccfe74804166ad2204ea02c072d79341cf75e7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506455"
---
# <a name="governanceschedule-resource-type"></a>governanceSchedule リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)のスケジュールを表します。 役割の割り当て要求の場合、スケジュールは、役割の割り当て操作を実行するタイミング、役割の割り当てを停止するタイミング、および役割の割り当て操作を実行する頻度を制御します。 



## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|startDateTime|DateTimeOffset|役割の割り当ての開始時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|endDateTime|DateTimeOffset|役割の割り当ての終了時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。 *注: 値がの場合`null`は、永続的な割り当てを示します。*|
|type|String|役割の割り当てスケジュールの種類。 現時点`Once`でのみサポートされています。
|duration|期間|役割の割り当ての期間。 これは、TimeSpan の形式です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSchedule"
}-->

```json
{
  "duration": "String (timespan)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceschedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
