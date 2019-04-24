---
title: FilterDatetime リソースの種類
description: 値をフィルター処理するときに日付をフィルター処理する方法を表します。
localization_priority: Normal
ms.openlocfilehash: ad4341e13eadc911377ec7b9859d6a31305fadf8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506442"
---
# <a name="filterdatetime-resource-type"></a>FilterDatetime リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

値をフィルター処理するときに日付をフィルター処理する方法を表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|date|string|データをフィルターをかけるための ISO8601 形式の日付です。|
|specificity|string|データを保持するのに、日付をどの程度詳細に使用するか。たとえば、date が 2005-04-02 で "month" に設定した場合、フィルター操作では 2005 年 4 月の日付データを含むすべての行が保持されます。可能な値は、`Year`、`Monday`、`Day`、`Hour`、`Minute`、`Second` です。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/filterdatetime.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
