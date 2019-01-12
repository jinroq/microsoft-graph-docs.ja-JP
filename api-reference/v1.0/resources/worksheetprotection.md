---
title: WorksheetProtection リソースの種類
description: シート オブジェクトの保護を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c8a719d1be9f21edf1bef82d2aa058b45bbf2df8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984235"
---
# <a name="worksheetprotection-resource-type"></a>WorksheetProtection リソースの種類

シート オブジェクトの保護を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[WorksheetProtection を取得する](../api/worksheetprotection-get.md) | [WorkbookWorksheetProtection](worksheetprotection.md) |worksheetProtection オブジェクトのプロパティと関係を読み取ります。|
|[Protect](../api/worksheetprotection-protect.md)|なし|ワークシートを保護します。ワークシートが保護されている場合はスローします。|
|[Unprotect](../api/worksheetprotection-unprotect.md)|なし|ワークシートの保護を解除します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|options|[WorkbookWorksheetProtectionOptions](worksheetprotectionoptions.md)|シートの保護のオプション。読み取り専用。|
|protected|ブール値|ワークシートが保護されているかどうかを示します。読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": true,
  "options": { "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
