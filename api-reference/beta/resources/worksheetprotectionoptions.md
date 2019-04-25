---
title: WorksheetProtectionOptions リソースの種類
description: シート保護のオプションを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e32e41eb46cc5af98f6d9aeffcf470e22fbad349
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523722"
---
# <a name="worksheetprotectionoptions-resource-type"></a>WorksheetProtectionOptions リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

シート保護のオプションを表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowAutoFilter|ブール値|自動フィルター機能の使用を可能にするワークシート保護オプションを表します。|
|allowDeleteColumns|ブール値|列の削除を可能にするワークシート保護オプションを表します。|
|allowDeleteRows|ブール値|行の削除を可能にするワークシート保護オプションを表します。|
|allowFormatCells|ブール値|セルの書式設定を可能にするワークシート保護オプションを表します。|
|allowFormatColumns|ブール値|列の書式設定を可能にするワークシート保護オプションを表します。|
|allowFormatRows|ブール値|行の書式設定を可能にするワークシート保護オプションを表します。|
|allowInsertColumns|ブール値|列の挿入を可能にするワークシート保護オプションを表します。|
|allowInsertHyperlinks|ブール値|ハイパーリンクの挿入を可能にするワークシート保護オプションを表します。|
|allowInsertRows|ブール値|行の挿入を可能にするワークシート保護オプションを表します。|
|allowPivotTables|ブール値|ピボット テーブル機能の使用を可能にするワークシート保護オプションを表します。|
|allowSort|ブール値|並ベ替え機能の使用を可能にするワークシート保護オプションを表します。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheetProtectionOptions"
}-->

```json
{
  "allowAutoFilter": true,
  "allowDeleteColumns": true,
  "allowDeleteRows": true,
  "allowFormatCells": true,
  "allowFormatColumns": true,
  "allowFormatRows": true,
  "allowInsertColumns": true,
  "allowInsertHyperlinks": true,
  "allowInsertRows": true,
  "allowPivotTables": true,
  "allowSort": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "WorksheetProtectionOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/worksheetprotectionoptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
