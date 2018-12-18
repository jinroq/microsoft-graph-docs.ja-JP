---
title: WorksheetProtectionOptions リソースの種類
description: シート保護のオプションを表します。
author: lumine2008
ms.openlocfilehash: d7217c825e1ac1fef297882ddf984bc94b10cc12
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335190"
---
# <a name="worksheetprotectionoptions-resource-type"></a>WorksheetProtectionOptions リソースの種類

シート保護のオプションを表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
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
  "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions"
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
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtectionOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->